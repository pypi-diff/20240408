# Comparing `tmp/AqOrg-0.1.8.tar.gz` & `tmp/AqOrg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AqOrg-0.1.8.tar", last modified: Sat May  8 00:27:50 2021, max compression
+gzip compressed data, was "dist\AqOrg-0.1.9.tar", last modified: Mon May 24 21:17:04 2021, max compression
```

## Comparing `AqOrg-0.1.8.tar` & `AqOrg-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2021-05-08 00:27:50.000000 AqOrg-0.1.8/
-drwxrwxrwx   0        0        0        0 2021-05-08 00:27:50.000000 AqOrg-0.1.8/AqOrg/
--rw-rw-rw-   0        0        0    36111 2021-05-08 00:25:11.000000 AqOrg-0.1.8/AqOrg/AqOrg.py
--rw-rw-rw-   0        0        0       74 2021-05-08 00:25:12.000000 AqOrg-0.1.8/AqOrg/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-08 00:27:50.000000 AqOrg-0.1.8/AqOrg.egg-info/
--rw-rw-rw-   0        0        0     1513 2021-05-08 00:27:50.000000 AqOrg-0.1.8/AqOrg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2021-05-08 00:27:50.000000 AqOrg-0.1.8/AqOrg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-08 00:27:50.000000 AqOrg-0.1.8/AqOrg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-05-08 00:27:50.000000 AqOrg-0.1.8/AqOrg.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2021-05-08 00:27:50.000000 AqOrg-0.1.8/AqOrg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-05-08 00:27:50.000000 AqOrg-0.1.8/AqOrg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1513 2021-05-08 00:27:50.000000 AqOrg-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      896 2021-05-08 00:15:35.000000 AqOrg-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2021-05-08 00:27:50.000000 AqOrg-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      880 2021-05-08 00:10:19.000000 AqOrg-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2021-05-24 21:17:04.000000 AqOrg-0.1.9/
+drwxrwxrwx   0        0        0        0 2021-05-24 21:17:04.000000 AqOrg-0.1.9/AqOrg/
+-rw-rw-rw-   0        0        0    45118 2021-05-24 21:16:40.000000 AqOrg-0.1.9/AqOrg/AqOrg.py
+-rw-rw-rw-   0        0        0       74 2021-05-24 20:02:50.000000 AqOrg-0.1.9/AqOrg/__init__.py
+drwxrwxrwx   0        0        0        0 2021-05-24 21:17:04.000000 AqOrg-0.1.9/AqOrg.egg-info/
+-rw-rw-rw-   0        0        0     1513 2021-05-24 21:17:04.000000 AqOrg-0.1.9/AqOrg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2021-05-24 21:17:04.000000 AqOrg-0.1.9/AqOrg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-05-24 21:17:04.000000 AqOrg-0.1.9/AqOrg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-05-24 21:17:04.000000 AqOrg-0.1.9/AqOrg.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2021-05-24 21:17:04.000000 AqOrg-0.1.9/AqOrg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2021-05-24 21:17:04.000000 AqOrg-0.1.9/AqOrg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1513 2021-05-24 21:17:04.000000 AqOrg-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      896 2021-05-24 20:02:50.000000 AqOrg-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2021-05-24 21:17:04.000000 AqOrg-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      880 2021-05-24 20:03:57.000000 AqOrg-0.1.9/setup.py
```

### Comparing `AqOrg-0.1.8/AqOrg/AqOrg.py` & `AqOrg-0.1.9/AqOrg/AqOrg.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # for benson group additivity
 from pgradd.GroupAdd.Library import GroupLibrary
 import pgradd.ThermoChem
 
 def find_HKF(Gh=float('NaN'), V=float('NaN'), Cp=float('NaN'),
              Gf=float('NaN'), Hf=float('NaN'), Saq=float('NaN'),
-             charge=float('NaN'), J_to_cal=True):
+             charge=float('NaN'), J_to_cal=True, print_eq=False):
     
     """
     Estimate HKF parameters from standard state thermodynamic properties of an
     aqueous organic molecule.
     
     Parameters
     ----------
@@ -45,14 +45,18 @@
     
     charge : numeric
         The charge of the molecule.
     
     J_to_cal : bool, default True
         Should the output be calorie-based? kJ/mol will be converted to cal/mol
         and J/mol/K will be converted to cal/mol/K.
+    
+    print_eq : bool, default False
+        Print equations used in estimation? Equations are printed in the order
+        they are calculated.
         
     Returns
     ----------
     out : dict
         A dictonary of properties and parameters. These will either be
         Joule-based or calorie-based depending on the parameter `J_to_cal`.
     """
@@ -62,136 +66,186 @@
 
     # define YBorn (1/K)
     YBorn = -5.81*10**-5
 
     # define QBorn (1/bar)
     QBorn = 5.90*10**-7
 
-    # define XBorn (1/K^2)
+    # define XBorn (1/K**2)
     XBorn = -3.09*10**-7
+    
+    if print_eq:
+        print("eta = {} (angstroms*cal/mol), YBorn = {} (1/K), QBorn = {} (1/bar), XBorn = {} (1/K**2)\n".format(eta, YBorn, QBorn, XBorn))
 
     # define abs_protonBorn (cal/mol), mentioned in text after Eq 47 in Shock and Helgeson 1988
     abs_protonBorn = (0.5387 * 10**5)
+    if print_eq:
+        print("abs_protonBorn = (0.5387 * 10**5), mentioned in text after Eq 47 in Shock and Helgeson 1988\n")
+
 
     if not pd.isnull(Gh) and charge == 0:
 
-        # find omega*10^-5 (j/mol) if neutral and Gh available
+        # find omega*10**-5 (j/mol) if neutral and Gh available
         # Eq 8 in Plyasunov and Shock 2001
         HKFomega = 2.61+(324.1/(Gh-90.6))
+        if print_eq:
+            print("HKFomega = 2.61+(324.1/(Gh-90.6)), Eq 8 in Plyasunov and Shock 2001, omega*10**-5 (j/mol)\n")
 
     elif charge == 0:
 
-        # find omega*10^-5 (j/mol) if neutral and Gh unavailable
+        # find omega*10**-5 (j/mol) if neutral and Gh unavailable
         # Eq 61 in Shock and Helgeson 1990 for NONVOLATILE neutral organic species
-        HKFomega = (10 ^ -5)*((-1514.4*(Saq/4.184)) + (0.34*10**5))*4.184
+        HKFomega = (10**-5)*((-1514.4*(Saq/4.184)) + (0.34*10**5))*4.184
+        if print_eq:
+            print("HKFomega = (10**-5)*((-1514.4*(Saq/4.184)) + (0.34*10**5))*4.184, Eq 61 in Shock and Helgeson 1990, omega*10**-5 (j/mol)\n")
 
     elif charge != 0:
 
         # define alphaZ (described in text after Eq 59 in Shock and Helgeson 1990)
         if (abs(charge) == 1):
             alphaZ = 72
         elif (abs(charge) == 2):
             alphaZ = 141
         elif (abs(charge) == 3):
             alphaZ = 211
         elif (abs(charge) == 4):
             alphaZ = 286
         else:
             alphaZ = float('NaN')
-
+        if print_eq and alphaZ != float('NaN'):
+            print("alphaZ = {} because charge = {}, described in text after Eq 59 in Shock and Helgeson 1990\n".format(alphaZ, charge))
+            
         # define BZ
         BZ = ((-alphaZ*eta)/(YBorn*eta - 100)) - charge * \
             abs_protonBorn  # Eq 55 in Shock and Helgeson 1990
-
-        # find ion omega*10^-5, (J/mol) if charged
-        HKFomega = (10 ^ -5)*(-1514.4*(Saq/4.184) + BZ) * \
+        if print_eq:
+            print("BZ = ((-alphaZ*eta)/(YBorn*eta - 100)) - charge * abs_protonBorn, Eq 55 in Shock and Helgeson 1990\n")
+            
+        # find ion omega*10**-5, (J/mol) if charged
+        HKFomega = (10**-5)*(-1514.4*(Saq/4.184) + BZ) * \
             4.184  # Eq 58 in Shock and Helgeson 1990
+        if print_eq:
+            print("HKFomega = (10**-5)*(-1514.4*(Saq/4.184) + BZ) * 4.184, Eq 58 in Shock and Helgeson 1990, omega*10**-5, (J/mol)\n")
 
         ### METHOD FOR INORGANIC AQUEOUS ELECTROLYTES USING SHOCK AND HELGESON 1988:
 
         # find rej (angstroms), ions only
-        #rej <- ((charge^2)*(eta*YBorn-100))/((Saq/4.184)-71.5*abs(charge)) # Eqs 46+56+57 in Shock and Helgeson 1988
+        #rej <- ((charge**2)*(eta*YBorn-100))/((Saq/4.184)-71.5*abs(charge)) # Eqs 46+56+57 in Shock and Helgeson 1988
 
-        # find ion absolute omega*10^-5, (cal/mol)
-        #HKFomega_abs_ion <- (eta*(charge^2))/rej # Eq 45 in Shock and Helgeson 1988
+        # find ion absolute omega*10**-5, (cal/mol)
+        #HKFomega_abs_ion <- (eta*(charge**2))/rej # Eq 45 in Shock and Helgeson 1988
 
-        # find ion omega*10^-5, (J/mol)
-        #HKFomega2 <- (10^-5)*(HKFomega_abs_ion-(charge*abs_protonBorn))*4.184 # Eq 47 in Shock and Helgeson 1988
+        # find ion omega*10**-5, (J/mol)
+        #HKFomega2 <- (10**-5)*(HKFomega_abs_ion-(charge*abs_protonBorn))*4.184 # Eq 47 in Shock and Helgeson 1988
 
     else:
         HKFomega = float('NaN')
 
     # find delta V solvation (cm3/mol)
     # Eq 5 in Shock and Helgeson 1988, along with a conversion of 10 cm3 = 1 joule/bar
     V_solv = -(HKFomega/10**-5)*QBorn*10
+    if print_eq:
+        print("V_solv = -(HKFomega/10**-5)*QBorn*10, Eq 5 in Shock and Helgeson 1988, along with a conversion of 10 cm3 = 1 joule/bar, delta V solvation (cm3/mol)\n")
 
     # find delta V nonsolvation (cm3/mol)
     V_nonsolv = V - V_solv  # Eq 4 in Shock and Helgeson 1988
+    if print_eq:
+        print("V_nonsolv = V - V_solv, Eq 4 in Shock and Helgeson 1988, delta V nonsolvation (cm3/mol)\n")
 
     # find sigma (cm3/mol)
     HKFsigma = 1.11*V_nonsolv + 1.8  # Eq 87 in Shock and Helgeson
-
-    # find delta cp solvation (J/mol*K)
+    if print_eq:
+        print("HKFsigma = 1.11*V_nonsolv + 1.8, Eq 87 in Shock and Helgeson, sigma (cm3/mol)\n")
+        
+    # find delta Cp solvation (J/mol*K)
     # Eq 35 in Shock and Helgeson 1988 dCpsolv = omega*T*X
     cp_solv = ((HKFomega/10**-5)*298.15*XBorn)
-
-    # find delta cp nonsolvation (J/mol*K)
+    if print_eq:
+        print("cp_solv = ((HKFomega/10**-5)*298.15*XBorn), Eq 35 in Shock and Helgeson 1988, dCpsolv = omega*T*X, delta Cp solvation (J/mol*K)\n")
+        
+    # find delta Cp nonsolvation (J/mol*K)
     cp_nonsolv = Cp - cp_solv  # Eq 29 in Shock and Helgeson 1988
-
+    if print_eq:
+        print("cp_nonsolv = Cp - cp_solv, Eq 29 in Shock and Helgeson 1988, delta Cp nonsolvation (J/mol*K)\n")
+        
     if not pd.isnull(Gh) and charge == 0:
         # find a1*10 (j/mol*bar)
         # Eq 10 in Plyasunov and Shock 2001
         HKFa1 = (0.820-((1.858*10**-3)*(Gh)))*V
         # why is this different than Eq 16 in Sverjensky et al 2014? Regardless, results seem to be very close using this eq vs. Eq 16.
-
-        # find a2*10^-2 (j/mol)
+        if print_eq:
+            print("HKFa1 = (0.820-((1.858*10**-3)*(Gh)))*V, Eq 10 in Plyasunov and Shock 2001, a1*10 (j/mol*bar)\n")
+            
+        # find a2*10**-2 (j/mol)
         # Eq 11 in Plyasunov and Shock 2001
         HKFa2 = (0.648+((0.00481)*(Gh)))*V
-
-        # find a4*10^-4 (j*K/mol)
+        if print_eq:
+            print("HKFa2 = (0.648+((0.00481)*(Gh)))*V, Eq 11 in Plyasunov and Shock 2001, a2*10**-2 (j/mol)\n")
+            
+        # find a4*10**-4 (j*K/mol)
         # Eq 12 in Plyasunov and Shock 2001
         HKFa4 = 8.10-(0.746*HKFa2)+(0.219*Gh)
-
+        if print_eq:
+            print("HKFa4 = 8.10-(0.746*HKFa2)+(0.219*Gh), Eq 12 in Plyasunov and Shock 2001, a4*10**-4 (j*K/mol)\n")
+            
     elif charge != 0:
         # find a1*10 (j/mol*bar)
         # Eq 16 in Sverjensky et al 2014, after Plyasunov and Shock 2001, converted to J/mol*bar. This equation is used in the DEW model since it works for charged and noncharged species up to 60kb
         HKFa1 = (0.1942*V_nonsolv + 1.52)*4.184
-
-        # find a2*10^-2 (j/mol)
-        # Eq 8 in Shock and Helgeson, rearranged to solve for a2*10^-2. Sigma is divided by 41.84 due to the conversion of 41.84 cm3 = cal/bar
+        if print_eq:
+            print("HKFa1 = (0.1942*V_nonsolv + 1.52)*4.184, Eq 16 in Sverjensky et al 2014, after Plyasunov and Shock 2001, converted to J/mol*bar, a1*10 (j/mol*bar)\n")
+            
+        # find a2*10**-2 (j/mol)
+        # Eq 8 in Shock and Helgeson, rearranged to solve for a2*10**-2. Sigma is divided by 41.84 due to the conversion of 41.84 cm3 = cal/bar
         HKFa2 = (10**-2)*(((HKFsigma/41.84) -
                         ((HKFa1/10)/4.184))/(1/(2601)))*4.184
-
-        # find a4*10^-4 (j*K/mol)
-        # Eq 88 in Shock and Helgeson, solve for a4*10^-4
+        if print_eq:
+            print("HKFa2 = (10**-2)*(((HKFsigma/41.84) - ((HKFa1/10)/4.184))/(1/(2601)))*4.184, Eq 8 in Shock and Helgeson, rearranged to solve for a2*10**-2 (j/mol). Sigma is divided by 41.84 due to the conversion of 41.84 cm3 = cal/bar\n")
+            
+        # find a4*10**-4 (j*K/mol)
+        # Eq 88 in Shock and Helgeson, solve for a4*10**-4
         HKFa4 = (10**-4)*(-4.134*(HKFa2/4.184)-27790)*4.184
-
+        if print_eq:
+            print("HKFa4 = (10**-4)*(-4.134*(HKFa2/4.184)-27790)*4.184, Eq 88 in Shock and Helgeson, a4*10**-4 (j*K/mol)\n")
+            
     else:
         HKFa1 = float('NaN')
         HKFa2 = float('NaN')
         HKFa3 = float('NaN')
-
-    # find c2*10^-4 (j*K/mol)
+        if print_eq:
+            print("HKF parameters a1, a2, and a3 could not be estimated.\n")
+           
+    # find c2*10**-4 (j*K/mol)
     if not pd.isnull(Gh) and charge == 0:
         HKFc2 = 21.4+(0.849*Gh)  # Eq 14 in Plyasunov and Shock 2001
+        if print_eq:
+            print("HKFc2 = 21.4+(0.849*Gh), Eq 14 in Plyasunov and Shock 2001, c2*10**-4 (j*K/mol)\n")
     elif not pd.isnull(Cp) and charge != 0:
         # Eq 89 in Shock and Helgeson 1988
         HKFc2 = (0.2037*(Cp/4.184) - 3.0346)*4.184
+        if print_eq:
+            print("HKFc2 = (0.2037*(Cp/4.184) - 3.0346)*4.184, Eq 89 in Shock and Helgeson 1988, c2*10**-4 (j*K/mol)\n")
     else:
         HKFc2 = float('NaN')
-
+        if print_eq:
+            print("HKF parameter c2 could not be estimated.")
+            
     # find c1 (j/mol*K)
     # Eq 31 in Shock and Helgeson 1988, rearranged to solve for c1
     HKFc1 = cp_nonsolv-(((HKFc2)/10**-4)*(1/(298.15-228))**2)
-
+    if print_eq:
+        print("HKFc1 = cp_nonsolv-(((HKFc2)/10**-4)*(1/(298.15-228))**2), Eq 31 in Shock and Helgeson 1988, rearranged to solve for c1 (j/mol*K)\n")
+            
     # find a3 (j*K/mol*bar)
     # Eq 11 in Shock and Helgeson 1988, rearranged to solve for a3. V is divided by 10 due to the conversion of 10 cm3 = J/bar
     HKFa3 = (((V/10)-(HKFa1/10)-((HKFa2/10**-2)/2601) +
             ((HKFomega/10**-5)*QBorn))/(1/(298.15-228)))-((HKFa4/10**-4)/2601)
-
+    if print_eq:
+        print("HKFa3 = (((V/10)-(HKFa1/10)-((HKFa2/10**-2)/2601) + ((HKFomega/10**-5)*QBorn))/(1/(298.15-228)))-((HKFa4/10**-4)/2601), Eq 11 in Shock and Helgeson 1988, rearranged to solve for a3 (j*K/mol*bar). V is divided by 10 due to the conversion of 10 cm3 = J/bar\n")
+            
     if J_to_cal:
         conv = 4.184
     else:
         conv = 1
 
     out = {
         "G": (Gf/conv)*1000,
@@ -210,41 +264,125 @@
         "Vsolv": V_solv,
         "Vnonsolv": V_nonsolv,
         "sigma": HKFsigma}
 
     return out
 
 
-def find_HKF_test():
+def find_HKF_test(print_eq=False):
     
     """
     Test the HKF estimation function by regenerating published values.
+    
+    Parameters
+    ----------
+    print_eq : bool, default False
+        Print equations used in estimation?
     """
     
-    print("phenolate", find_HKF(Gh=-80.74, V=68.16, Cp=105, Gf=5.795, Hf=-129.0, Saq=76.6, charge=-1))
-    print("phenolate, 1988 method", find_HKF(Gh=float('NaN'), V=68.16, Cp=105, Gf=5.795, Hf=-129.0, Saq=76.6, charge=-1))
-
-    print("Be+2", find_HKF(V=-25.4, Cp=-1.3*4.184, Gf=(-83500*4.184) /
-                                1000, Hf=(-91500*4.184)/1000, Saq=-55.7*4.184, charge=2))
-    print("NH4+", find_HKF(V=18.13, Cp=15.74*4.184, Gf=(-18990*4.184) /
-                                1000, Hf=(-31850*4.184)/1000, Saq=26.57*4.184, charge=1))
-    print("Li+", find_HKF(V=-0.87, Cp=14.2*4.184, Gf=(-69933*4.184) /
-                               1000, Hf=(-66552*4.184)/1000, Saq=2.70*4.184, charge=1))
+    #print("\n---------------------------------------------")
+    
+#     print("phenolate\n---------")
+#     print("Input parameters:")
+#     print("Gh=-80.74, V=68.16, Cp=105, Gf=5.795, Hf=-129.0, Saq=76.6, charge=-1\n")
+#     out = find_HKF(Gh=-80.74, V=68.16, Cp=105,
+#                    Gf=5.795, Hf=-129.0, Saq=76.6, charge=-1,
+#                    print_eq=print_eq)
+    
+#     print("phenolate, 1988 method\n---------")
+#     print("Input parameters:")
+#     print("Gh=float('NaN'), V=68.16, Cp=105, Gf=5.795, Hf=-129.0, Saq=76.6, charge=-1\n")
+#     out = find_HKF(Gh=float('NaN'), V=68.16, Cp=105,
+#                    Gf=5.795, Hf=-129.0, Saq=76.6, charge=-1,
+#                    print_eq=print_eq)
+
+#     print("Be+2\n---------")
+#     print("Input parameters:")
+#     print("V=-25.4, Cp=-1.3*4.184, Gf=(-83500*4.184)/1000, Hf=(-91500*4.184)/1000, Saq=-55.7*4.184, charge=2\n")
+#     out = find_HKF(V=-25.4, Cp=-1.3*4.184, Gf=(-83500*4.184)/1000,
+#                    Hf=(-91500*4.184)/1000, Saq=-55.7*4.184, charge=2,
+#                    print_eq=print_eq)
+    
+#     print("NH4+\n---------")
+#     print("Input parameters:")
+#     print("V=18.13, Cp=15.74*4.184, Gf=(-18990*4.184)/1000, Hf=(-31850*4.184)/1000, Saq=26.57*4.184, charge=1\n")
+#     out = find_HKF(V=18.13, Cp=15.74*4.184, Gf=(-18990*4.184)/1000,
+#                    Hf=(-31850*4.184)/1000, Saq=26.57*4.184, charge=1,
+#                    print_eq=print_eq)
+    
+#     print("Li+\n---------")
+#     print("Input parameters:")
+#     print("V=-0.87, Cp=14.2*4.184, Gf=(-69933*4.184)/1000, Hf=(-66552*4.184)/1000, Saq=2.70*4.184, charge=1\n")
+#     out = find_HKF(V=-0.87, Cp=14.2*4.184, Gf=(-69933*4.184)/1000,
+#                    Hf=(-66552*4.184)/1000, Saq=2.70*4.184, charge=1,
+#                    print_eq=print_eq)
 
     # Compare to table 4 of Plyasunov and Shock 2001
     # (may be slightly different due to using Eq 16 in Sverjensky et al 2014 for calculating a1)
-    print("SO2", find_HKF(Gh=-0.51, V=39.0,
-                               Cp=146, charge=0, J_to_cal=False))
-    print("Pyridine", find_HKF(Gh=-11.7, V=77.1,
-                                    Cp=306, charge=0, J_to_cal=False))
-    print("1,4-Butanediol", find_HKF(Gh=-37.7, V=88.23,
-                                          Cp=347, charge=0, J_to_cal=False))
-    print("beta-alanine", find_HKF(Gh=-74, V=58.7,
-                                        Cp=76, charge=0, J_to_cal=False))
-
+    print("PLYASUNOV AND SHOCK 2001, TABLE 4\n---------------------------------------------")
+    
+    print("SO2\n---------")
+    print("Input parameters:")
+    print("Gh=-0.51, V=39.0, Cp=146, charge=0, J_to_cal=False\n")
+    out = find_HKF(Gh=-0.51, V=39.0, Cp=146, charge=0, J_to_cal=False, print_eq=print_eq)
+    pub = {"omega":"-0.95", "a1":"32.02", "a2":"25.17",
+           "a3":"18.71", "a4":"-10.79", "c1":"93.2", "c2":"20.97"}
+    print("Published: {}, \tCalculated: {}, \tomega*10**-5".format(pub["omega"], round(out["omega"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta1*10".format(pub["a1"], round(out["a1"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta2*10**-2".format(pub["a2"], round(out["a2"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta3".format(pub["a3"], round(out["a3"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta4*10**-4".format(pub["a4"], round(out["a4"], 2)))
+    print("Published: {}, \tCalculated: {}, \tc1".format(pub["c1"], round(out["c1"], 1)))
+    print("Published: {}, \tCalculated: {}, \tc2*10**-4".format(pub["c2"], round(out["c2"], 2)))
+    print("")
+    
+    print("Pyridine\n---------")
+    print("Input parameters:")
+    print("Gh=-11.7, V=77.1, Cp=306, charge=0, J_to_cal=False\n")
+    out = find_HKF(Gh=-11.7, V=77.1, Cp=306, charge=0, J_to_cal=False, print_eq=print_eq)
+    pub = {"omega":"-0.56", "a1":"64.89", "a2":"45.62",
+           "a3":"69.94", "a4":"-28.50", "c1":"278.1", "c2":"11.47"}
+    print("Published: {}, \tCalculated: {}, \tomega*10**-5".format(pub["omega"], round(out["omega"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta1*10".format(pub["a1"], round(out["a1"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta2*10**-2".format(pub["a2"], round(out["a2"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta3".format(pub["a3"], round(out["a3"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta4*10**-4".format(pub["a4"], round(out["a4"], 2)))
+    print("Published: {}, \tCalculated: {}, \tc1".format(pub["c1"], round(out["c1"], 1)))
+    print("Published: {}, \tCalculated: {}, \tc2*10**-4".format(pub["c2"], round(out["c2"], 2)))
+    print("")
+    
+    print("1,4-Butanediol\n---------")
+    print("Input parameters:")
+    print("Gh=-37.7, V=88.23, Cp=347, charge=0, J_to_cal=False\n")
+    out = find_HKF(Gh=-37.7, V=88.23, Cp=347, charge=0, J_to_cal=False, print_eq=print_eq)
+    pub = {"omega":"0.08", "a1":"78.50", "a2":"41.17",
+           "a3":"76.32", "a4":"-30.87", "c1":"369.2", "c2":"-10.61"}
+    print("Published: {}, \tCalculated: {}, \tomega*10**-5".format(pub["omega"], round(out["omega"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta1*10".format(pub["a1"], round(out["a1"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta2*10**-2".format(pub["a2"], round(out["a2"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta3".format(pub["a3"], round(out["a3"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta4*10**-4".format(pub["a4"], round(out["a4"], 2)))
+    print("Published: {}, \tCalculated: {}, \tc1".format(pub["c1"], round(out["c1"], 1)))
+    print("Published: {}, \tCalculated: {}, \tc2*10**-4".format(pub["c2"], round(out["c2"], 2)))
+    print("")
+    
+    print("beta-alanine\n---------")
+    print("Input parameters:")
+    print("Gh=-74, V=58.7, Cp=76, charge=0, J_to_cal=False\n")
+    out = find_HKF(Gh=-74, V=58.7, Cp=76, charge=0, J_to_cal=False, print_eq=print_eq)
+    pub = {"omega":"0.64", "a1":"56.17", "a2":"17.14",
+           "a3":"54.55", "a4":"-20.90", "c1":"165.5", "c2":"-41.43"}
+    print("Published: {}, \tCalculated: {}, \tomega*10**-5".format(pub["omega"], round(out["omega"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta1*10".format(pub["a1"], round(out["a1"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta2*10**-2".format(pub["a2"], round(out["a2"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta3".format(pub["a3"], round(out["a3"], 2)))
+    print("Published: {}, \tCalculated: {}, \ta4*10**-4".format(pub["a4"], round(out["a4"], 2)))
+    print("Published: {}, \tCalculated: {}, \tc1".format(pub["c1"], round(out["c1"], 1)))
+    print("Published: {}, \tCalculated: {}, \tc2*10**-4".format(pub["c2"], round(out["c2"], 2)))
+    print("")
 
 def find_sigfigs(x):
     
     '''
     Get the number of significant digits in a string representing a number up to
     eight digits long.
 
@@ -694,15 +832,15 @@
                 # derive Sh, entropy of hydration, in J/mol K
                 if prop == "Sh":
                     # Entropy calculated from S = (G-H)/(-Tref)
                     mol_prop = (float(self.Gh) - float(self.Hh))/(-298.15)
                     mol_prop = mol_prop*1000 # convert kJ/molK to J/molK
 
                     # propagate error from Gh and Hh to estimate Sh error.
-                    # equation used: Sh_err = Sh*sqrt((Gh_err/Gh)^2 + (Hh_err/Hh)^2)
+                    # equation used: Sh_err = Sh*sqrt((Gh_err/Gh)**2 + (Hh_err/Hh)**2)
                     Gh_err_float = float(self.Gh_err)/float(self.Gh)
                     Hh_err_float = float(self.Hh_err)/float(self.Hh)
                     mol_err = abs(mol_prop)*math.sqrt(Gh_err_float**2 + Hh_err_float**2)
 
                     # check whether Gh or Hh as the fewest sigfigs
                     sf = min([find_sigfigs(self.Gh), find_sigfigs(self.Hh)])
```

### Comparing `AqOrg-0.1.8/AqOrg.egg-info/PKG-INFO` & `AqOrg-0.1.9/AqOrg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AqOrg
-Version: 0.1.8
+Version: 0.1.9
 Summary: Estimate thermodynamic properties of aqueous organic compounds
 Home-page: UNKNOWN
 Author: Grayson Boyer
 Author-email: gmboyer@asu.edu
 License: UNKNOWN
 Description: # AqOrg
```

### Comparing `AqOrg-0.1.8/PKG-INFO` & `AqOrg-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AqOrg
-Version: 0.1.8
+Version: 0.1.9
 Summary: Estimate thermodynamic properties of aqueous organic compounds
 Home-page: UNKNOWN
 Author: Grayson Boyer
 Author-email: gmboyer@asu.edu
 License: UNKNOWN
 Description: # AqOrg
```

### Comparing `AqOrg-0.1.8/README.md` & `AqOrg-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `AqOrg-0.1.8/setup.py` & `AqOrg-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AqOrg",
-    version="0.1.8",
+    version="0.1.9",
     author="Grayson Boyer",
     author_email="gmboyer@asu.edu",
     description="Estimate thermodynamic properties of aqueous organic compounds",
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={},
     packages=['AqOrg'],
```

