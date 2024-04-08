# Comparing `tmp/graymatter_swissknife-1.1.6.tar.gz` & `tmp/graymatter_swissknife-1.1.7.tar.gz`

## Comparing `graymatter_swissknife-1.1.6.tar` & `graymatter_swissknife-1.1.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/images/GM_models_from_GEM.png
--rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/images/gm_swissknife_square_low_res.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/__init__.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/__about__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/__init__.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/__main__.py
--rw-r--r--   0        0        0    11291 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/estimate_model.py
--rw-r--r--   0        0        0    10866 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/estimate_model_noiseless.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/find_model.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/microstructure_models.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/GEM/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/GEM/gem.py
--rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/GEM/gem_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/GEM/functions/__init__.py
--rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/__init__.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/nexi.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/nexi_dot.py
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/nexi_rm.py
--rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/smex.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/smex_rm.py
--rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
--rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDI/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDI/sandi.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDI/sandi_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDI/functions/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDIX/__init__.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDIX/sandix.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
--rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/parameters/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/parameters/acq_parameters.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/parameters/mist_parameters.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/parameters/save_parameters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/rice_noise/__init__.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/rice_noise/rice_mean.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/struct_functions/__init__.py
--rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
--rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/nls/__init__.py
--rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/nls/gridsearch.py
--rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/nls/nls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/powderaverage/__init__.py
--rw-r--r--   0        0        0    12678 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/powderaverage/powderaverage.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/xgboost/define_xgboost_model.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/src/graymatter_swissknife/xgboost/generate_dataset.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/generate_phantom.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/test_estimate_model.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/test_estimate_model_noiseless.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/mask.nii.gz
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/phantom.bval
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/phantom.nii.gz
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/phantom.td
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/powderaverage_ref.bval
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/powderaverage_ref.td
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_sigma_ref.nii.gz
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
--rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/models/test_nexi_functions.py
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/models/test_rician_mean.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/tests/graymatter_swissknife/xgboost/test_generate_dataset.py
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/.gitignore
--rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/LICENSE
--rw-r--r--   0        0        0     9407 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/README.md
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/pyproject.toml
--rw-r--r--   0        0        0    10444 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/images/GM_models_from_GEM.png
+-rw-r--r--   0        0        0   586456 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/images/gm_swissknife_square_low_res.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/__about__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/__init__.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/__main__.py
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/estimate_model.py
+-rw-r--r--   0        0        0    10912 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/estimate_model_noiseless.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/find_model.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/microstructure_models.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/gem.py
+-rw-r--r--   0        0        0     4214 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/gem_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/functions/__init__.py
+-rw-r--r--   0        0        0    23322 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/__init__.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi.py
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_dot.py
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_rm.py
+-rw-r--r--   0        0        0     2429 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/smex.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/smex_rm.py
+-rw-r--r--   0        0        0    36906 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py
+-rw-r--r--   0        0        0    11231 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/__init__.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/sandi.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/sandi_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/functions/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/__init__.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/sandix.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/sandix_rm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/functions/__init__.py
+-rw-r--r--   0        0        0     7372 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/acq_parameters.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/mist_parameters.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/save_parameters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/rice_noise/__init__.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/rice_noise/rice_mean.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/__init__.py
+-rw-r--r--   0        0        0    16385 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py
+-rw-r--r--   0        0        0    21687 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/__init__.py
+-rw-r--r--   0        0        0     6721 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/gridsearch.py
+-rw-r--r--   0        0        0     6962 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/nls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/powderaverage/__init__.py
+-rw-r--r--   0        0        0    10247 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/powderaverage/powderaverage.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/apply_xgboost_model.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/define_xgboost_model.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/generate_dataset.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/generate_phantom.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/test_estimate_model.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/test_estimate_model_noiseless.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/lowb_noisemap.nii.gz
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/mask.nii.gz
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/mask_upd_ref.nii.gz
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/normalized_sigma_ref.nii.gz
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/phantom.bval
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/phantom.nii.gz
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/phantom.td
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/powderaverage_ref.bval
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/powderaverage_ref.td
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_de_ref.nii.gz
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_di_ref.nii.gz
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_f_ref.nii.gz
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_de_ref.nii.gz
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_di_ref.nii.gz
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_f_ref.nii.gz
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/models_ref/nexi_t_ex_ref.nii.gz
+-rw-r--r--   0        0        0     4077 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/models/test_nexi_functions.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/models/test_rician_mean.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/powderaverage/test_powderaverage.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/tests/graymatter_swissknife/xgboost/test_generate_dataset.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/.gitignore
+-rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/LICENSE
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/README.md
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0    10829 2020-02-02 00:00:00.000000 graymatter_swissknife-1.1.7/PKG-INFO
```

### Comparing `graymatter_swissknife-1.1.6/images/GM_models_from_GEM.png` & `graymatter_swissknife-1.1.7/images/GM_models_from_GEM.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/images/gm_swissknife_square_low_res.png` & `graymatter_swissknife-1.1.7/images/gm_swissknife_square_low_res.png`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/estimate_model.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/estimate_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,23 +67,24 @@
     logging.basicConfig(level=logging.INFO, format='%(message)s')  # Set the logging level to INFO or desired level
 
     # Create the output directory if it does not exist
     if not os.path.exists(out_path):
         os.makedirs(out_path)
 
     # Convert into powder average
-    powder_average_path, updated_bvals_path, updated_td_path = powder_average(
+    powder_average_path, updated_bvals_path, updated_td_path, updated_mask_path = powder_average(
         dwi_path, bvals_path, td_path, mask_path, out_path, debug=debug
     )
     # NEXI with Rician Mean correction
     normalized_sigma_filename = normalize_sigma(dwi_path, lowb_noisemap_path, bvals_path, out_path)
     powder_average_signal_npz_filename = save_data_as_npz(
         powder_average_path,
         updated_bvals_path,
         updated_td_path,
+        updated_mask_path,
         out_path,
         normalized_sigma_filename=normalized_sigma_filename,
         debug=debug,
     )
 
     # Load the powder average signal, normalized sigma, b-values and diffusion time (acquisition parameters)
     powder_average_signal_npz = np.load(powder_average_signal_npz_filename)
@@ -176,15 +177,15 @@
         np.savez_compressed(
             f'{out_path}/{microstruct_model.name.lower()}_estimations.npz',
             estimations=estimations,
             estimation_init=estimation_init,
         )
 
     # Save the model parameters as nifti
-    save_estimations_as_nifti(estimations, microstruct_model, powder_average_path, mask_path, out_path, optimization_method)
+    save_estimations_as_nifti(estimations, microstruct_model, powder_average_path, updated_mask_path, out_path, optimization_method)
 
 
 if __name__ == '__main__':
     # Parse arguments
     parser = argparse.ArgumentParser(
         description='Estimate the NEXI model parameters for a given set of preprocessed '
         'signals, providing the b-values and diffusion time.'
```

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/estimate_model_noiseless.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/estimate_model_noiseless.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,20 @@
     logging.basicConfig(level=logging.INFO, format='%(message)s')  # Set the logging level to INFO or desired level
 
     # Create the output directory if it does not exist
     if not os.path.exists(out_path):
         os.makedirs(out_path)
 
     # Convert into powder average
-    powder_average_path, updated_bvals_path, updated_td_path = powder_average(
+    powder_average_path, updated_bvals_path, updated_td_path, updated_mask_path = powder_average(
         dwi_path, bvals_path, td_path, mask_path, out_path, debug=debug
     )
     # Model without Rician Mean correction
     powder_average_signal_npz_filename = save_data_as_npz(
-        powder_average_path, updated_bvals_path, updated_td_path, out_path, debug=debug
+        powder_average_path, updated_bvals_path, updated_td_path, updated_mask_path, out_path, debug=debug
     )
 
     # Load the powder average signal, b-values and diffusion time (acquisition parameters)
     powder_average_signal_npz = np.load(powder_average_signal_npz_filename)
     signal = powder_average_signal_npz['signal']
     voxel_nb = len(signal)
     bvals = powder_average_signal_npz['b']
@@ -167,15 +167,15 @@
         np.savez_compressed(
             f'{out_path}/{microstruct_model.name.lower()}_estimations.npz',
             estimations=estimations,
             estimation_init=estimation_init,
         )
 
     # Save the NEXI model parameters as nifti
-    save_estimations_as_nifti(estimations, microstruct_model, powder_average_path, mask_path, out_path, optimization_method)
+    save_estimations_as_nifti(estimations, microstruct_model, powder_average_path, updated_mask_path, out_path, optimization_method)
 
 
 if __name__ == '__main__':
     # Parse arguments
     parser = argparse.ArgumentParser(
         description='Estimate the NEXI model parameters for a given set of preprocessed '
         'signals, providing the b-values and diffusion time.'
```

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/find_model.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/find_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/microstructure_models.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/microstructure_models.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/GEM/gem.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/GEM/gem_rm.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/gem_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/GEM/functions/scipy_gem.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/nexi.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/nexi_dot.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_dot_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/nexi_rm.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/nexi_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/smex.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/smex_rm.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/smex_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_nexi_dot.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/NEXI/functions/scipy_smex.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDI/sandi.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDI/sandi_rm.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/sandi_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDI/functions/scipy_sandi.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDIX/sandix.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDIX/sandix_rm.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/sandix_rm.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/SANDIX/functions/scipy_sandix.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/parameters/acq_parameters.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/acq_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/parameters/mist_parameters.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/mist_parameters.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/parameters/save_parameters.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/parameters/save_parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     param_map_shape = mask.shape
 
     param_names = model.param_names
     # Remove the last parameter (sigma) from the parameter names if the model has a Rician mean correction
     if model.has_rician_mean_correction:
         param_names = param_names[:-1]
     for i, param_name in enumerate(param_names):
-        param_map = np.zeros(param_map_shape)
+        param_map = np.zeros(param_map_shape) * np.nan
         param_map[mask] = estimations[:, i]
         param_map_nifti = nib.Nifti1Image(param_map, aff, hdr)
         if optimization_method == 'nls':
             nib.save(param_map_nifti, f'{out_path}/{model.name.lower()}_{param_name.lower()}.nii.gz')
             logging.info(f'{model.name.lower()}_{param_name.lower()}.nii.gz saved in {out_path}')
         else:
             nib.save(param_map_nifti, f'{out_path}/{optimization_method}_{model.name.lower()}_{param_name.lower()}.nii.gz')
```

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/rice_noise/rice_mean.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/rice_noise/rice_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/scipy_cylinder.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/models/struct_functions/scipy_sphere.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/nls/gridsearch.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/gridsearch.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/nls/nls.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/nls/nls.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/powderaverage/powderaverage.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/powderaverage/powderaverage.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,81 +32,71 @@
     updated_td_path : str
         Path to the updated diffusion times (in ms) txt file.
     """
 
     powder_average_filename = f'{out_path}/powderaverage_dwi.nii.gz'
     updated_bvals_path = f'{out_path}/powderaverage.bval'
     updated_td_path = f'{out_path}/powderaverage.td'
+    updated_mask_path = f'{out_path}/updated_mask.nii.gz'
     # Re-split the image into different diffusion times
     dwi_image_nii = nib.load(dwi_path)
     dwi_image = dwi_image_nii.get_fdata()
     aff, hdr = dwi_image_nii.affine, dwi_image_nii.header
     tdvalues = np.loadtxt(td_path).astype(float)
     bvalues = np.loadtxt(bvals_path).astype(float)
-    # Convert the mask into booleans
-    if mask_path is not None:
-        mask = np.squeeze(nib.load(mask_path).get_fdata())
-    else:
-        mask = np.ones(dwi_image.shape[:-1])
-    # threshold for the mask (coulb also be 0.33)
-    # If you touch it, please change it also in save_parameters.py
-    mask_threshold = 0 
-    bool_mask = np.copy(mask) > mask_threshold 
     # Initialize powder average image, b-values and diffusion times
     pa_image = []
     pa_b = []
     pa_td = []
-    # Initialize nan mask
-    nan_mask = np.copy(bool_mask).astype(float)
     for td in np.unique(tdvalues):
         # Find b0s
         b0_selection = (tdvalues == td) & (bvalues == 0)
         nb_of_b0 = np.sum(b0_selection)
         assert nb_of_b0 != 0
         # Compute the mean of all b0 images to have one unique b0 image
         if nb_of_b0 > 1:
             b0_image = np.mean(dwi_image[..., b0_selection], axis=-1)
         else:
             b0_image = dwi_image[..., b0_selection][..., 0]
         # Convert eventual negative values
         b0_image = np.abs(b0_image)
-        # Update mask with the positions in the b0 images where the signal is equal to zero (to avoid div. by 0)
-        bool_mask = bool_mask & (b0_image != 0)
-        # Convert the boolean mask into a 1.0/nan mask to be easily multiplied
-        nan_mask = np.copy(bool_mask).astype(float)
-        nan_mask[bool_mask == 0] = np.nan
+        # Replace 0 in b0_image by np.nan
+        b0_image[b0_image == 0] = np.nan
         # Put the b0 image, b and td inside the lists
-        pa_image.append((b0_image != 0).astype(float) * nan_mask)
+        pa_image.append((~np.isnan(b0_image)).astype(float))
         pa_b.append(0)
         pa_td.append(td)
         # Sort the unique (non-zero) b-values per diffusion time
         nonzero_b = np.sort(np.unique(bvalues[tdvalues == td]))[1:]
-        # Generate a np.nan mask for the normalization to avoid division by 0
-        nan_mask = np.copy(bool_mask).astype(float)
-        nan_mask[bool_mask == 0] = np.nan
         for b in nonzero_b:
             selection = (tdvalues == td) & (bvalues == b)
             norm_image = np.mean(dwi_image[..., selection], axis=-1)
             # Compute the normalization inside the mask
-            norm_image = np.divide(norm_image * nan_mask, b0_image * nan_mask)
+            norm_image = np.divide(norm_image, b0_image)
             # Add all features to the lists
             pa_image.append(norm_image)
             pa_b.append(b)
             pa_td.append(td)
-            # Update mask with the values where the diffusion-weighted signal were lower than the b0 image
-            # bool_mask = bool_mask & (norm_image < 1)
-            # nan_mask = np.copy(bool_mask).astype(float)
-            # nan_mask[bool_mask == 0] = np.nan
     # Convert the list of powder averaged images into numpy array
     pa_image = np.stack(pa_image, axis=-1)
+
+    # APPLY MASK AND UPDATE MASK WITH NAN VALUES FROM THE POWDER AVERAGED IMAGE
+    # Convert the mask into booleans
+    if mask_path is not None:
+        mask = np.squeeze(nib.load(mask_path).get_fdata())
+    else:
+        mask = np.ones(dwi_image.shape[:-1])
+    # threshold for the mask (coulb also be 0.33)
+    # If you touch it, please change it also in save_parameters.py
+    mask_threshold = 0 
     # Make sure the mask is the intersection between the original mask 
     # and where the powder averaged image is not NaN
-    bool_mask = (mask > mask_threshold) & (~np.isnan(np.sum(pa_image, axis=-1)))
-    # Reapply the last updated mask to every volume
-    pa_image = nan_mask[..., None] * pa_image
+    bool_mask = (mask > mask_threshold) & (~np.any(np.isnan(pa_image), axis=-1))
+    # Replace values in pa_image outside of the mask by NaN
+    pa_image[~bool_mask, :] = np.nan
     # Get rid of extreme values
     pa_image = np.clip(pa_image, 0, 1)
 
     # Check and convert b-values from s/mm² to ms/µm² if provided in s/mm²
     if np.max(pa_b) > 500:
         # Warn that the b-values were probably not in ms/µm²:
         warnings.warn(
@@ -126,89 +116,31 @@
 
     # Save without the b = 0 ms/µm² images
     without_b0 = np.array(pa_b) != 0
     pa_img_no_b0 = pa_image[..., without_b0]
     pa_b_no_b0 = np.array(pa_b)[without_b0]
     pa_td_no_b0 = np.array(pa_td)[without_b0]
     powder_average_nii = nib.Nifti1Image(pa_img_no_b0, affine=aff, header=hdr)
+    bool_mask_nii = nib.Nifti1Image(bool_mask, affine=aff, header=hdr)
     nib.save(powder_average_nii, powder_average_filename)
+    nib.save(bool_mask_nii, updated_mask_path)
     if debug:
         logging.info(
             f"Without b0s, image shape : {pa_img_no_b0.shape}  with maximum value of {np.nanmax(pa_img_no_b0)}"
         )
         logging.info(f"b-values :{pa_b_no_b0}")
         logging.info(f"td values :{pa_td_no_b0}")
 
     # Save b-values and diffusion times
     np.savetxt(updated_bvals_path, pa_b_no_b0, fmt='%1.3f')
     np.savetxt(updated_td_path, pa_td_no_b0, fmt='%1.3f')
 
     logging.info("Powder average finished !")
 
-    return powder_average_filename, updated_bvals_path, updated_td_path
-
-
-# Save to npz
-def save_powder_average_as_npz(dwi_path, bvals_path, td_path, small_delta, out_path, debug=False):
-    """
-    Save the powder averaged image, b-values and diffusion times in a npz file
-
-    Parameters
-    ----------
-    dwi_path : str
-        Path to the dwi image
-    bvals_path : str
-        Path to the b-values file
-    td_path : str
-        Path to the diffusion times file
-    small_delta : float
-        Small delta value in ms
-    out_path : str
-        Path to the output folder
-    debug : bool
-        If True, print some information for debugging
-
-    Returns
-    -------
-    powder_average_signal_npz_filename : str
-        Path to the npz file containing the powder averaged image, b-values and diffusion times
-    """
-    powder_average_signal_npz_filename = f'{out_path}/powderaverage_signal.npz'
-    # Extract the powder-averaged image, b-values and diffusion times
-    pa_image_nii = nib.load(dwi_path)
-    pa_image = np.clip(pa_image_nii.get_fdata(), 0, 1)
-    bval = np.loadtxt(bvals_path)
-    tdval = np.loadtxt(td_path)
-
-    if debug:
-        logging.info("Sanity Check")
-        logging.info(f"b-values : {bval}")
-        logging.info(f"diffusion times : {tdval}")
-        logging.info(f"small delta : {small_delta}")
-
-    # Initialize the extraction of the signal values where there is no NaN
-    mask = pa_image.sum(axis=-1) > 0
-    mask = mask.astype(bool) & np.invert(np.isnan(mask))
-    locations = np.array(np.where(mask)).T  # (N, 3)
-    signal = pa_image[mask, :]
-
-    if debug:
-        logging.info(f"Is there any nan ? {np.isnan(signal).sum()}")
-        logging.info(f"Meaningful signal shape : {signal.shape}")
-
-    np.savez_compressed(
-        powder_average_signal_npz_filename,
-        signal=signal,
-        b=bval,
-        td=tdval,
-        small_delta=small_delta,
-        locations=locations,
-        img_shape=pa_image.shape[0:3],
-    )
-    return powder_average_signal_npz_filename
+    return powder_average_filename, updated_bvals_path, updated_td_path, updated_mask_path
 
 
 def normalize_sigma(dwi_path, lowb_noisemap_path, bvals_path, out_path):
     """
     Normalize the noisemap by the b0 image
 
     Parameters
@@ -233,32 +165,38 @@
     b0 = dwi_nii.get_fdata()[..., bval == 0]
     b0 = np.mean(b0, axis=-1)
     # Load the noisemap
     noisemap = noisemap_nii.get_fdata()
     if noisemap.ndim >= 4:
         noisemap = np.squeeze(noisemap)
     assert noisemap.ndim == 3, "Noisemap should be 3D"
+    # Replace the 0 and negative values by NaN in b0
+    b0[b0 <= 0] = np.nan
     # Normalize the noisemap (sigma)
     norm_sigma = np.divide(noisemap, b0)
     # Sigma should be strictly higher than 0, we also clip it at 100
     norm_sigma = np.clip(norm_sigma, 1e-9, 100)
+    # Replace the NaN values by the lowest value of the noisemap
+    norm_sigma[np.isnan(norm_sigma)] = np.nanmin(norm_sigma)
+    # Replace the values higher than 99 by NaN
     norm_sigma[norm_sigma > 99] = np.nan
     # Save the normalized sigma map
     normalized_sigma_nii = nib.Nifti1Image(norm_sigma, affine=aff, header=hdr)
     normalized_sigma_filename = f'{out_path}/normalized_sigma.nii.gz'
     nib.save(normalized_sigma_nii, normalized_sigma_filename)
 
     return normalized_sigma_filename
 
 
 def save_data_as_npz(
     powder_average_filename,
     bvals_path,
     td_path,
-    out_path,
+    updated_mask_path,
+    out_path, 
     normalized_sigma_filename=None,
     small_delta=None,
     debug=False,
 ):
     """
     Save the powder averaged image, b-values and diffusion times in a npz file
 
@@ -285,24 +223,23 @@
     """
     powder_average_signal_npz_filename = f'{out_path}/powderaverage_signal.npz'
     # Extract the powder-averaged image, b-values and diffusion times
     pa_image_nii = nib.load(powder_average_filename)
     pa_image = np.clip(pa_image_nii.get_fdata(), 0, 1)
     bval = np.loadtxt(bvals_path)
     tdval = np.loadtxt(td_path)
+    mask = nib.load(updated_mask_path).get_fdata()
 
     if debug:
         logging.info("Sanity Check")
         logging.info(f"b-values : {bval}")
         logging.info(f"diffusion times : {tdval}")
 
     # Initialize the extraction of the signal values where there is no NaN
-    mask = pa_image.sum(axis=-1) > 0
-    mask = mask.astype(bool) & np.invert(np.isnan(mask))
-    locations = np.array(np.where(mask)).T  # (N, 3)
+    mask = mask.astype(bool) & (~np.any(np.isnan(pa_image), axis=-1))
     signal = pa_image[mask, :]
 
     if debug:
         logging.info(f"Is there any NaN in the signal ? {np.isnan(np.sum(signal))}")
         logging.info(f"Meaningful signal shape : {signal.shape}")
         logging.info(f"Mask shape : {mask.shape}")
 
@@ -315,21 +252,19 @@
         np.savez_compressed(
             powder_average_signal_npz_filename,
             signal=signal,
             sigma=sigma,
             b=bval,
             td=tdval,
             small_delta=small_delta,
-            locations=locations,
-            img_shape=pa_image.shape[0:3],
+            mask=mask
         )
     else:
         np.savez_compressed(
             powder_average_signal_npz_filename,
             signal=signal,
             b=bval,
             td=tdval,
             small_delta=small_delta,
-            locations=locations,
-            img_shape=pa_image.shape[0:3],
+            mask=mask
         )
     return powder_average_signal_npz_filename
```

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/xgboost/apply_xgboost_model.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/apply_xgboost_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/xgboost/define_xgboost_model.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/define_xgboost_model.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/src/graymatter_swissknife/xgboost/generate_dataset.py` & `graymatter_swissknife-1.1.7/src/graymatter_swissknife/xgboost/generate_dataset.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/tests/graymatter_swissknife/generate_phantom.py` & `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/generate_phantom.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/tests/graymatter_swissknife/test_estimate_model.py` & `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/test_estimate_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,30 +28,32 @@
     )
 
     powder_average_filename = 'tests/graymatter_swissknife/data/nexi_rice_mean/powderaverage_dwi.nii.gz'
     bval_filename = 'tests/graymatter_swissknife/data/nexi_rice_mean/powderaverage.bval'
     td_filename = 'tests/graymatter_swissknife/data/nexi_rice_mean/powderaverage.td'
     powder_average_npz_filename = 'tests/graymatter_swissknife/data/nexi_rice_mean/powderaverage_signal.npz'
     sigma_filename = 'tests/graymatter_swissknife/data/nexi_rice_mean/normalized_sigma.nii.gz'
+    updated_mask_filename = 'tests/graymatter_swissknife/data/nexi_rice_mean/updated_mask.nii.gz'
 
     assert np.allclose(
         nib.load(powder_average_filename).get_fdata(),
         nib.load('tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz').get_fdata(),
         equal_nan=True,
     )
     assert np.allclose(np.loadtxt(bval_filename), np.loadtxt('tests/graymatter_swissknife/data/powderaverage_ref.bval'))
     assert np.allclose(np.loadtxt(td_filename), np.loadtxt('tests/graymatter_swissknife/data/powderaverage_ref.td'))
 
     os.remove(powder_average_filename)
     os.remove(bval_filename)
     os.remove(td_filename)
     os.remove(powder_average_npz_filename)
     os.remove(sigma_filename)
+    os.remove(updated_mask_filename)
 
-    parameters = ["t_ex", "di", "de", "f", "sigma"]
+    parameters = ["t_ex", "di", "de", "f"]  # , "sigma"]
     for param in parameters:
         param_filename = f'tests/graymatter_swissknife/data/nexi_rice_mean/nexi_rice_mean_{param}.nii.gz'
         param_ref_filename = f'tests/graymatter_swissknife/data/models_ref/nexi_rice_mean_{param}_ref.nii.gz'
         assert np.allclose(
             nib.load(param_filename).get_fdata(), nib.load(param_ref_filename).get_fdata(), equal_nan=True
         )
         os.remove(param_filename)
```

### Comparing `graymatter_swissknife-1.1.6/tests/graymatter_swissknife/test_estimate_model_noiseless.py` & `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/test_estimate_model_noiseless.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,29 @@
         debug=False,
     )
 
     powder_average_filename = 'tests/graymatter_swissknife/data/nexi/powderaverage_dwi.nii.gz'
     bval_filename = 'tests/graymatter_swissknife/data/nexi/powderaverage.bval'
     td_filename = 'tests/graymatter_swissknife/data/nexi/powderaverage.td'
     powder_average_npz_filename = 'tests/graymatter_swissknife/data/nexi/powderaverage_signal.npz'
+    updated_mask_filename = 'tests/graymatter_swissknife/data/nexi/updated_mask.nii.gz'
 
     assert np.allclose(
         nib.load(powder_average_filename).get_fdata(),
         nib.load('tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz').get_fdata(),
         equal_nan=True,
     )
     assert np.allclose(np.loadtxt(bval_filename), np.loadtxt('tests/graymatter_swissknife/data/powderaverage_ref.bval'))
     assert np.allclose(np.loadtxt(td_filename), np.loadtxt('tests/graymatter_swissknife/data/powderaverage_ref.td'))
 
     os.remove(powder_average_filename)
     os.remove(bval_filename)
     os.remove(td_filename)
     os.remove(powder_average_npz_filename)
+    os.remove(updated_mask_filename)
 
     parameters = ["t_ex", "di", "de", "f"]
     for param in parameters:
         param_filename = f'tests/graymatter_swissknife/data/nexi/nexi_{param}.nii.gz'
         param_ref_filename = f'tests/graymatter_swissknife/data/models_ref/nexi_{param}_ref.nii.gz'
         assert np.allclose(
             nib.load(param_filename).get_fdata(), nib.load(param_ref_filename).get_fdata(), equal_nan=True
```

### Comparing `graymatter_swissknife-1.1.6/tests/graymatter_swissknife/data/phantom.nii.gz` & `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/data/phantom.nii.gz`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/tests/graymatter_swissknife/models/test_nexi_functions.py` & `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/models/test_nexi_functions.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/tests/graymatter_swissknife/models/test_rician_mean.py` & `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/models/test_rician_mean.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/tests/graymatter_swissknife/powderaverage/test_powderaverage.py` & `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/powderaverage/test_powderaverage.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,32 +9,38 @@
 sys.path.append(project_root)
 
 from src.graymatter_swissknife.powderaverage.powderaverage import powder_average, normalize_sigma
 
 
 def test_powder_average():
 
-    powder_average_filename, bval_filename, td_filename = powder_average(
+    powder_average_filename, bval_filename, td_filename, mask_filename = powder_average(
         'tests/graymatter_swissknife/data/phantom.nii.gz',
         'tests/graymatter_swissknife/data/phantom.bval',
         'tests/graymatter_swissknife/data/phantom.td',
         'tests/graymatter_swissknife/data/mask.nii.gz',
         'tests/graymatter_swissknife/data',
         debug=False,
     )
     assert np.allclose(
         nib.load(powder_average_filename).get_fdata(),
         nib.load('tests/graymatter_swissknife/data/powderaverage_dwi_ref.nii.gz').get_fdata(),
         equal_nan=True,
     )
+    assert np.allclose(
+        nib.load(mask_filename).get_fdata(),
+        nib.load('tests/graymatter_swissknife/data/mask_upd_ref.nii.gz').get_fdata(),
+        equal_nan=True,
+    )
     assert np.allclose(np.loadtxt(bval_filename), np.loadtxt('tests/graymatter_swissknife/data/powderaverage_ref.bval'))
     assert np.allclose(np.loadtxt(td_filename), np.loadtxt('tests/graymatter_swissknife/data/powderaverage_ref.td'))
     os.remove(powder_average_filename)
     os.remove(bval_filename)
     os.remove(td_filename)
+    os.remove(mask_filename)
 
 
 def test_normalize_sigma():
     # sys.path.append('../')
     normalized_sigma_filename = normalize_sigma(
         'tests/graymatter_swissknife/data/phantom.nii.gz',
         'tests/graymatter_swissknife/data/lowb_noisemap.nii.gz',
```

### Comparing `graymatter_swissknife-1.1.6/tests/graymatter_swissknife/xgboost/test_generate_dataset.py` & `graymatter_swissknife-1.1.7/tests/graymatter_swissknife/xgboost/test_generate_dataset.py`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/.gitignore` & `graymatter_swissknife-1.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/LICENSE` & `graymatter_swissknife-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/README.md` & `graymatter_swissknife-1.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,24 +22,26 @@
 - [Citation](#citation)
 - [License](#license)
 
 
 ## Installation
 
 ```console
+pip install numpy nibabel tqdm joblib scipy xgboost scikit-learn
 pip install graymatter_swissknife
 ```
 
 ## Usage
 
 ### Estimate Gray Matter microstructure model parameters
 
 To estimate any gray matter model parameters with Nonlinear Least Squares using the graymatter_swissknife package, you can use the estimate_model function. This function takes several parameters that you need to provide in order to perform the estimation accurately.
 
 ```
+from graymatter_swissknife import estimate_model
 estimate_model(model_name, dwi_path, bvals_path, td_path, small_delta, lowb_noisemap_path, out_path)
 ```
 
 `model_name`: Choose your gray matter model between `'Nexi'` (or `'Nexi_Narrow_Pulses_Approximation'`), `'Smex'` (or `'Nexi_Wide_Pulses'`), `'Sandi'`, `'Sandix'` and `'Gem'`.
 
 `dwi_path`: The path to the diffusion-weighted image (DWI) data in NIfTI format. This data contains the preprocessed diffusion-weighted volumes acquired from your imaging study.
 
@@ -51,31 +53,31 @@
 
 `lowb_noisemap_path`: The path to the noisemap calculated using only the small b-values (b < 2 ms/µm²) and Marchenko-Pastur principal component analysis (MP-PCA) denoising. This noisemap is used to calculate the signal-to-noise ratio (SNR) of the data.
 
 `out_path`: The folder where the estimated parameters will be saved as output.
 
 **Additional options:**
 
-`mask_path` (Recommended): The mask path, if the analysis concerns a specific portion of the DWI images. The mask can be in 3 dimensions, or must be able to be squeezed in only 3 dimensions.
+`mask_path` (**Recommended**): The mask path, if the analysis concerns a specific portion of the DWI images. The mask can be in 3 dimensions, or must be able to be squeezed in only 3 dimensions.
 
 `fixed_parameters` (Optional): Allows to fix some parameters of the model if not set to None. Tuple of fixed parameters for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). Example of use: Fix Di to 2.0µm²/ms and De to 1.0µm²/ms in the NEXI model by specifying fixed_parameters=(None, 2.0 , 1.0, None)
 
 `adjust_parameter_limits` (Optional): Allows to redefine some parameter limits of the model if not set to None. Tuple of adjusted parameter limits for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). This will have no effect on the fixed parameters (if set in fixed_parameters). Example of use: Fix Di limits to (1.5-2.5)µm²/ms and De to (0.5-1.5)µm²/ms in the NEXI model by specifying fixed_parameters=(None, (1.5, 2.5) , (0.5, 1.5), None)
 
 `n_cores`: Number of cores to use for the parallelization. If -1, all available cores are used. The default is -1.
 
 `debug`: Debug mode. The default is False.
 
-## Fast XGBoost Estimation:
+### Fast XGBoost Estimation (Artificial Intelligence)
 
-The Non-Linear Least Squares method is preferred for the most accurate estimates. However, this method takes a long time to fit. To analyze large cohorts, we could recommend training an XGBoost model to learn the model on the given parameter limits, then applying this trained model to the entire cohort. To achieve this, we use the following arguments:
+The Non-Linear Least Squares method is preferred for the most accurate estimates. However, this method takes a long time to fit. For the analysis of extensive cohorts, we propose employing an XGBoost model to learn the microstructure model on the given parameter limits, then applying this trained XGBoost model to the entire cohort. For example, employing this approach enables the execution of a NEXI analysis on an entire cohort within a timeframe of less than **10 minutes**, provided that the scan parameters remain consistent across the cohort. To achieve this, we use the following arguments:
 
 `optimization_method`: To use XGBoost, set this setting to `'xgboost'`. The default is `'nls'`.
 
-`xgboost_model_path`: If the model is not yet trained, this setting indicates where the model and its weights will be saved. If the model is already trained, then this setting must indicate where it will be saved. The default is None. If `optimization_method` is set to `'xgboost'`, this setting will be required.
+`xgboost_model_path`: If the model is not yet trained, this setting indicates where the model and its weights will be saved. If the model is already trained, then this setting must indicate where it is saved. The default is None. If `optimization_method` is set to `'xgboost'`, this setting will be required.
 
 `retrain_xgboost` (Optional): Boolean to indicate if you wish to overwrite the model already trained and saved at the address indicated in xgboost_model_path. The default and recommended setting is False. The safest way is to delete the saved file yourself.
 
 ### Gray Matter microstructure models description from the Generalized Exchange Model
 
 ![](images/GM_models_from_GEM.png)
```

### Comparing `graymatter_swissknife-1.1.6/pyproject.toml` & `graymatter_swissknife-1.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `graymatter_swissknife-1.1.6/PKG-INFO` & `graymatter_swissknife-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: graymatter_swissknife
-Version: 1.1.6
+Version: 1.1.7
 Summary: Gray Matter Swiss Knife : Generalized Exchange Model estimators for diffusion MRI
 Project-URL: Documentation, https://github.com/QuentinUhl/graymatter_swissknife#readme
 Project-URL: Issues, https://github.com/QuentinUhl/graymatter_swissknife/issues
 Project-URL: Source, https://github.com/QuentinUhl/graymatter_swissknife
 Author-email: Quentin Uhl <quentin.uhl@gmail.com>, "Ileana O. Jelescu" <ileana.jelescu@chuv.ch>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -45,24 +45,26 @@
 - [Citation](#citation)
 - [License](#license)
 
 
 ## Installation
 
 ```console
+pip install numpy nibabel tqdm joblib scipy xgboost scikit-learn
 pip install graymatter_swissknife
 ```
 
 ## Usage
 
 ### Estimate Gray Matter microstructure model parameters
 
 To estimate any gray matter model parameters with Nonlinear Least Squares using the graymatter_swissknife package, you can use the estimate_model function. This function takes several parameters that you need to provide in order to perform the estimation accurately.
 
 ```
+from graymatter_swissknife import estimate_model
 estimate_model(model_name, dwi_path, bvals_path, td_path, small_delta, lowb_noisemap_path, out_path)
 ```
 
 `model_name`: Choose your gray matter model between `'Nexi'` (or `'Nexi_Narrow_Pulses_Approximation'`), `'Smex'` (or `'Nexi_Wide_Pulses'`), `'Sandi'`, `'Sandix'` and `'Gem'`.
 
 `dwi_path`: The path to the diffusion-weighted image (DWI) data in NIfTI format. This data contains the preprocessed diffusion-weighted volumes acquired from your imaging study.
 
@@ -74,31 +76,31 @@
 
 `lowb_noisemap_path`: The path to the noisemap calculated using only the small b-values (b < 2 ms/µm²) and Marchenko-Pastur principal component analysis (MP-PCA) denoising. This noisemap is used to calculate the signal-to-noise ratio (SNR) of the data.
 
 `out_path`: The folder where the estimated parameters will be saved as output.
 
 **Additional options:**
 
-`mask_path` (Recommended): The mask path, if the analysis concerns a specific portion of the DWI images. The mask can be in 3 dimensions, or must be able to be squeezed in only 3 dimensions.
+`mask_path` (**Recommended**): The mask path, if the analysis concerns a specific portion of the DWI images. The mask can be in 3 dimensions, or must be able to be squeezed in only 3 dimensions.
 
 `fixed_parameters` (Optional): Allows to fix some parameters of the model if not set to None. Tuple of fixed parameters for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). Example of use: Fix Di to 2.0µm²/ms and De to 1.0µm²/ms in the NEXI model by specifying fixed_parameters=(None, 2.0 , 1.0, None)
 
 `adjust_parameter_limits` (Optional): Allows to redefine some parameter limits of the model if not set to None. Tuple of adjusted parameter limits for the model. The tuple must have the same length as the number of parameters of the model (with or without noise correction). This will have no effect on the fixed parameters (if set in fixed_parameters). Example of use: Fix Di limits to (1.5-2.5)µm²/ms and De to (0.5-1.5)µm²/ms in the NEXI model by specifying fixed_parameters=(None, (1.5, 2.5) , (0.5, 1.5), None)
 
 `n_cores`: Number of cores to use for the parallelization. If -1, all available cores are used. The default is -1.
 
 `debug`: Debug mode. The default is False.
 
-## Fast XGBoost Estimation:
+### Fast XGBoost Estimation (Artificial Intelligence)
 
-The Non-Linear Least Squares method is preferred for the most accurate estimates. However, this method takes a long time to fit. To analyze large cohorts, we could recommend training an XGBoost model to learn the model on the given parameter limits, then applying this trained model to the entire cohort. To achieve this, we use the following arguments:
+The Non-Linear Least Squares method is preferred for the most accurate estimates. However, this method takes a long time to fit. For the analysis of extensive cohorts, we propose employing an XGBoost model to learn the microstructure model on the given parameter limits, then applying this trained XGBoost model to the entire cohort. For example, employing this approach enables the execution of a NEXI analysis on an entire cohort within a timeframe of less than **10 minutes**, provided that the scan parameters remain consistent across the cohort. To achieve this, we use the following arguments:
 
 `optimization_method`: To use XGBoost, set this setting to `'xgboost'`. The default is `'nls'`.
 
-`xgboost_model_path`: If the model is not yet trained, this setting indicates where the model and its weights will be saved. If the model is already trained, then this setting must indicate where it will be saved. The default is None. If `optimization_method` is set to `'xgboost'`, this setting will be required.
+`xgboost_model_path`: If the model is not yet trained, this setting indicates where the model and its weights will be saved. If the model is already trained, then this setting must indicate where it is saved. The default is None. If `optimization_method` is set to `'xgboost'`, this setting will be required.
 
 `retrain_xgboost` (Optional): Boolean to indicate if you wish to overwrite the model already trained and saved at the address indicated in xgboost_model_path. The default and recommended setting is False. The safest way is to delete the saved file yourself.
 
 ### Gray Matter microstructure models description from the Generalized Exchange Model
 
 ![](images/GM_models_from_GEM.png)
```

