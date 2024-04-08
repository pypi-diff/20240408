# Comparing `tmp/panpipelines-0.9.7.tar.gz` & `tmp/panpipelines-0.9.8.tar.gz`

## Comparing `panpipelines-0.9.7.tar` & `panpipelines-0.9.8.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-0.9.7/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-0.9.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/README.md
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/run_pan250.sh
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/config/license.txt
--rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/config/pan250.config
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/config/pan250_eddyparams.json
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PAN250_Deployment/config/credentials/credentials.json
--rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/README.md
--rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/run_pan_slurm.sh
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/README.md
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
--rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/ArterialAtlasLabels.txt
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/README.md
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
--rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
--rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVCORT/README.md
--rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVSUBCORT/README.md
--rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/README.md
--rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
--rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
--rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
--rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/JHU-labels_index.txt
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/JHU-tracts_index.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/README.md
--rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
--rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/README.md
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/XTRACT_index.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
--rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
--rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
--rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/README.md
--rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/fs_default.txt
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/README.md
--rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
--rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/group_template.pbs
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/participant_template.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_cpu.pbs
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_gpu.pbs
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
--rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/eddy_params.json
--rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/eddy_params_cpu.json
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/freebash.sh
--rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/license.txt
--rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/panpipeconfig_expanded_slurm.config
--rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/panpipeconfig_slurm.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.7/deployment/config/credentials/credentials.json
--rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-0.9.7/example/run_pan_example.sh
--rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-0.9.7/example/config/panpipeconfig_example.config
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.7/example/config/credentials/credentials_example.json
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/Factory.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/__init__.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/group_subjects.py
--rwxr-xr-x   0        0        0    18168 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pan_processing.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/single_subject.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/version.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/__init__.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/antstransform.py
--rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/aslprep.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/atlascreate.py
--rw-r--r--   0        0        0    21152 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/basil.py
--rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/collate_csv_group.py
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/collate_csv_single.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/dummy.py
--rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/fmriprep.py
--rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/freesurfer.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/fslanat.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/glm_randomize_group.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/lst.py
--rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/noddi.py
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/parse_textdata.py
--rw-r--r--   0        0        0    14261 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/preproc.py
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/qsiprep.py
--rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/roi_extract.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/roi_mean_group.py
--rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/roi_mean_single.py
--rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/nodes/tensor.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/aslprep_panpipeline.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/basil_panpipeline.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/collatecsv_panpipeline.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/dummy_panpipeline.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/fmriprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/freesurfer_panpipeline.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/lst_panpipeline.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/noddi_panpipeline.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/preproc_panpipeline.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/qsiprep_panpipeline.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/roiextract_panpipeline.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/tensor_panpipeline.py
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/textmeasures_panpipeline.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/pipelines/volmeasures_panpipeline.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/__init__.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/aslprep_panscript.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/fmriprep_panscript.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/mne_make_surfaces.py
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/pancontainer_panscript.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/panscript.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/scripts/sdcflows_fieldmap.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/utils/__init__.py
--rw-r--r--   0        0        0    31963 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/utils/transformer.py
--rw-r--r--   0        0        0    71325 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/utils/util_functions.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/__init__.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/aslprep_workflow.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/basil_workflow.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/collatecsv_workflow.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/collatecsvgroup_workflow.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/dummy_workflow.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/fmriprep_workflow.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/freesurfer_workflow.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/lst_workflow.py
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/noddi_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/preproc_workflow.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/qsiprep_workflow.py
--rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/roiextract_workflow.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/tensor_workflow.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/textmeasures_workflow.py
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-0.9.7/src/panpipelines/workflows/volmeasures_workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-0.9.7/tests/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-0.9.7/tests/test_PANFactory.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-0.9.7/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-0.9.7/LICENSE
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-0.9.7/README.md
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.7/pyproject.toml
--rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 panpipelines-0.9.8/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 panpipelines-0.9.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/README.md
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/run_pan250.sh
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_long.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_medium.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_small.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_tiny.pbs
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_highpri_verylong.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_small.pbs
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_cpu_tiny.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/config/license.txt
+-rw-r--r--   0        0        0    10449 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/config/pan250.config
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/config/pan250_eddyparams.json
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PAN250_Deployment/config/credentials/credentials.json
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/README.md
+-rwxr-xr-x   0        0        0     1471 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/run_pan_slurm.sh
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/AAL3v1_1mm_index.txt
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/README.md
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0   119500 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json
+-rw-r--r--   0        0        0    38695 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/eye.mat
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/ArterialAtlasLabels.txt
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/README.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/res-01_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/res-02_atlas-Arterial_dseg.tsv
+-rw-r--r--   0        0        0   182712 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0   182309 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json
+-rw-r--r--   0        0        0    37861 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVCORT/README.md
+-rwxr-xr-x   0        0        0   138203 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVSUBCORT/HarvardOxford-Subcortical_index.txt
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVSUBCORT/README.md
+-rwxr-xr-x   0        0        0   166519 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/README.md
+-rwxr-xr-x   0        0        0    14105 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt
+-rwxr-xr-x   0        0        0    12646 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt
+-rw-r--r--   0        0        0  1316983 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot
+-rw-r--r--   0        0        0  1316984 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/JHU-labels_index.txt
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/JHU-tracts_index.txt
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/README.md
+-rwxr-xr-x   0        0        0    47474 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz
+-rwxr-xr-x   0        0        0    47922 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/XTRACT_index.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0   191828 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json
+-rw-r--r--   0        0        0    42696 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz
+-rw-r--r--   0        0        0   196623 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz
+-rwxr-xr-x   0        0        0    89181 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/README.md
+-rwxr-xr-x   0        0        0    10131 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/fs_a2009s.txt
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/fs_default.txt
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/README.md
+-rwxr-xr-x   0        0        0    14879 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt
+-rwxr-xr-x   0        0        0    13454 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/group_template.pbs
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/participant_template.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_cpu.pbs
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_cpu_fmriprep.pbs
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_cpu_highpri.pbs
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_cpu_highpri_fmriprep.pbs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_gpu.pbs
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_gpu_highpri.pbs
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/batch_scripts/headers/slurm_gpu_windfall.pbs
+-rwxr-xr-x   0        0        0      384 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/eddy_params.json
+-rwxr-xr-x   0        0        0      379 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/eddy_params_cpu.json
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/freebash.sh
+-rwxr-xr-x   0        0        0       66 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/license.txt
+-rw-r--r--   0        0        0    23977 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/panpipeconfig_expanded_slurm.config
+-rw-r--r--   0        0        0    28701 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/panpipeconfig_slurm.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.8/deployment/config/credentials/credentials.json
+-rwxr-xr-x   0        0        0      215 2020-02-02 00:00:00.000000 panpipelines-0.9.8/example/run_pan_example.sh
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 panpipelines-0.9.8/example/config/panpipeconfig_example.config
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 panpipelines-0.9.8/example/config/credentials/credentials_example.json
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/Factory.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/__init__.py
+-rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/group_subjects.py
+-rwxr-xr-x   0        0        0    18596 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pan_processing.py
+-rw-r--r--   0        0        0     9022 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/single_subject.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/version.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/__init__.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/antstransform.py
+-rw-r--r--   0        0        0     6406 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/aslprep.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/atlascreate.py
+-rw-r--r--   0        0        0    22503 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/basil.py
+-rw-r--r--   0        0        0     7549 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/collate_csv_group.py
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/collate_csv_single.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/dummy.py
+-rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/fmriprep.py
+-rw-r--r--   0        0        0    10720 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/freesurfer.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/fslanat.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/glm_randomize_group.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/lst.py
+-rw-r--r--   0        0        0     6175 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/noddi.py
+-rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/parse_textdata.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/preproc.py
+-rw-r--r--   0        0        0     7806 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/qsiprep.py
+-rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/roi_extract.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/roi_mean_group.py
+-rw-r--r--   0        0        0    11130 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/roi_mean_single.py
+-rw-r--r--   0        0        0    10201 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/nodes/tensor.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/aslprep_panpipeline.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/basil_panpipeline.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/collatecsv_panpipeline.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/dummy_panpipeline.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/fmriprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/freesurfer_panpipeline.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/lst_panpipeline.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/noddi_panpipeline.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/preproc_panpipeline.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/qsiprep_panpipeline.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/roiextract_panpipeline.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/tensor_panpipeline.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/textmeasures_panpipeline.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/pipelines/volmeasures_panpipeline.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/__init__.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/aslprep_panscript.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/fmriprep_panscript.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/mne_make_surfaces.py
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/pancontainer_panscript.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/panscript.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/scripts/sdcflows_fieldmap.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/utils/__init__.py
+-rw-r--r--   0        0        0    31963 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/utils/transformer.py
+-rw-r--r--   0        0        0    73934 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/utils/util_functions.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/aslprep_workflow.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/basil_workflow.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/collatecsv_workflow.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/collatecsvgroup_workflow.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/dummy_workflow.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/fmriprep_workflow.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/freesurfer_workflow.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/lst_workflow.py
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/noddi_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/preproc_workflow.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/qsiprep_workflow.py
+-rw-r--r--   0        0        0     7525 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/roiextract_workflow.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/tensor_workflow.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/textmeasures_workflow.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 panpipelines-0.9.8/src/panpipelines/workflows/volmeasures_workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpipelines-0.9.8/tests/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 panpipelines-0.9.8/tests/test_PANFactory.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 panpipelines-0.9.8/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 panpipelines-0.9.8/LICENSE
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 panpipelines-0.9.8/README.md
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 panpipelines-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0    15188 2020-02-02 00:00:00.000000 panpipelines-0.9.8/PKG-INFO
```

### Comparing `panpipelines-0.9.7/.github/workflows/python-package.yml` & `panpipelines-0.9.8/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/.github/workflows/python-publish.yml` & `panpipelines-0.9.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/README.md` & `panpipelines-0.9.8/PAN250_Deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/run_pan250.sh` & `panpipelines-0.9.8/PAN250_Deployment/run_pan250.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/README.md` & `panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.8/PAN250_Deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/README.md` & `panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.8/PAN250_Deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/batch_scripts/group_template.pbs` & `panpipelines-0.9.8/PAN250_Deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/batch_scripts/participant_template.pbs` & `panpipelines-0.9.8/PAN250_Deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PAN250_Deployment/config/pan250.config` & `panpipelines-0.9.8/PAN250_Deployment/config/pan250.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/README.md` & `panpipelines-0.9.8/deployment/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/run_pan_slurm.sh` & `panpipelines-0.9.8/deployment/run_pan_slurm.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/AAL3v1_1mm_index.txt` & `panpipelines-0.9.8/deployment/atlas/AAL3/AAL3v1_1mm_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/README.md` & `panpipelines-0.9.8/deployment/atlas/AAL3/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv` & `panpipelines-0.9.8/deployment/atlas/AAL3/res-01_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv` & `panpipelines-0.9.8/deployment/atlas/AAL3/res-02_atlas-AAL3_dseg.tsv`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz` & `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/AAL3v1_1mm_MNI152NLin6Asym.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json` & `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz` & `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json` & `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz` & `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-AAL3_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh` & `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/convert.sh`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py` & `panpipelines-0.9.8/deployment/atlas/AAL3/MNI152NLin6Asym/Development/getTemplate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/Arterial/README.md` & `panpipelines-0.9.8/deployment/atlas/Arterial/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz` & `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/ArterialAtlas_int.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json` & `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json` & `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz` & `panpipelines-0.9.8/deployment/atlas/Arterial/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-Arterial_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt` & `panpipelines-0.9.8/deployment/atlas/HARVCORT/HarvardOxford-Cortical_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.8/deployment/atlas/HARVCORT/MNI152NLinAsym/HarvardOxford-cort-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.8/deployment/atlas/HARVSUBCORT/MNI152NLinAsym/HarvardOxford-sub-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/README.md` & `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt` & `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt` & `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/hcpmmp1_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot` & `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/lh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot` & `panpipelines-0.9.8/deployment/atlas/HCPMMP1_FREESURFER/rh.HCP-MMP1.annot`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/JHU/JHU-labels_index.txt` & `panpipelines-0.9.8/deployment/atlas/JHU/JHU-labels_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/JHU/JHU-tracts_index.txt` & `panpipelines-0.9.8/deployment/atlas/JHU/JHU-tracts_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz` & `panpipelines-0.9.8/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-labels-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz` & `panpipelines-0.9.8/deployment/atlas/JHU/MNI152NLinAsym/JHU-ICBM-tracts-maxprob-thr25-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/README.md` & `panpipelines-0.9.8/deployment/atlas/XTRACT/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/XTRACT_index.txt` & `panpipelines-0.9.8/deployment/atlas/XTRACT/XTRACT_index.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.8/deployment/atlas/XTRACT/res-01_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt` & `panpipelines-0.9.8/deployment/atlas/XTRACT/res-02_atlas-XTRACT_dseg.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json` & `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-01_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json` & `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.json`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz` & `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/tpl-MNI152NLin6Asym_res-02_atlas-XTRACT_dseg.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz` & `panpipelines-0.9.8/deployment/atlas/XTRACT/MNI152NLin6Asym/xtract-tract-atlases-maxprob5-1mm.nii.gz`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt` & `panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/FreeSurferColorLUT.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/fs_a2009s.txt` & `panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/fs_a2009s.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/freesurfer_atlas/fs_default.txt` & `panpipelines-0.9.8/deployment/atlas/freesurfer_atlas/fs_default.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt` & `panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_ordered.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt` & `panpipelines-0.9.8/deployment/atlas/hcpmmp1_subfields_atlas/hcpmmp1_subfields_original.txt`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/batch_scripts/group_template.pbs` & `panpipelines-0.9.8/deployment/batch_scripts/group_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/batch_scripts/participant_template.pbs` & `panpipelines-0.9.8/deployment/batch_scripts/participant_template.pbs`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/config/panpipeconfig_expanded_slurm.config` & `panpipelines-0.9.8/deployment/config/panpipeconfig_expanded_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/deployment/config/panpipeconfig_slurm.config` & `panpipelines-0.9.8/deployment/config/panpipeconfig_slurm.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/example/config/panpipeconfig_example.config` & `panpipelines-0.9.8/example/config/panpipeconfig_example.config`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/Factory.py` & `panpipelines-0.9.8/src/panpipelines/Factory.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/group_subjects.py` & `panpipelines-0.9.8/src/panpipelines/group_subjects.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from panpipelines import Factory
 
 LOGGER = logger_setup("panpipelines.group_subjects", logging.DEBUG)
 logger_addstdout(LOGGER, logging.INFO)
 
 panFactory = Factory.getPANFactory()
 
-def runGroupSubjects(participant_label, xnat_projects, session_label, pipeline, pipeline_class, pipeline_outdir, panpipe_labels,bids_dir,cred_user,cred_password, execution_json,analysis_level="group",panlabel=None):
+def runGroupSubjects(participant_label, xnat_projects, xnat_shared_projects, session_label, pipeline, pipeline_class, pipeline_outdir, panpipe_labels,bids_dir,cred_user,cred_password, execution_json,analysis_level="group",panlabel=None):
 
     # get parent directory
     if not panlabel:
         panlabel=os.path.basename(os.path.dirname(pipeline_outdir))
 
     pipeline_outdir=os.path.join(pipeline_outdir,"group")
     if not os.path.exists(pipeline_outdir):
@@ -103,15 +103,16 @@
 
     participants_file = getParams(panpipe_labels,"PARTICIPANTS_FILE")
     bids_dir = getParams(panpipe_labels,"BIDS_DIR")
 
     participant_labels = getParams(panpipe_labels,"GROUP_PARTICIPANTS_LABEL")
     xnat_projects = getParams(panpipe_labels,"GROUP_PARTICIPANTS_XNAT_PROJECT")
     session_labels = getParams(panpipe_labels,"GROUP_SESSION_LABEL")
+    xnat_shared_projects = getParams(panpipe_labels,"GROUP_PARTICIPANTS_XNAT_SHARED_PROJECT")
     
-    runGroupSubjects(participant_labels,xnat_projects, session_labels, pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level="group")
+    runGroupSubjects(participant_labels,xnat_projects, xnat_shared_projects, session_labels, pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level="group")
 
 
 
 # This is the standard boilerplate that calls the main() function.
 if __name__ == '__main__':
     main()
```

### Comparing `panpipelines-0.9.7/src/panpipelines/pan_processing.py` & `panpipelines-0.9.8/src/panpipelines/pan_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,14 +206,15 @@
 
     LOGGER.info(f"Pipelines to be processed : {pipelines}")
 
     projectmap = get_projectmap(participant_label, participants_file,session_labels=session_label,sessions_file=sessions_file,subject_exclusions=participant_exclusions)
     participant_list = projectmap[0]
     project_list  = projectmap[1]
     session_list = projectmap[2]
+    shared_project_list  = projectmap[3]
 
     # take snapshot of the runtime labels for all pipelines
     runtime_labels = panpipe_labels.copy()
 
     for pipeline in pipelines:
         LOGGER.info(f"Processing pipeline : {pipeline}")
         panpipe_labels = updateParams(panpipe_labels, "PIPELINE", pipeline)
@@ -255,18 +256,20 @@
             analysis_node = getParams(panpipe_labels,"ANALYSIS_NODE")
 
             if analysis_level == "group":
                 updateParams(panpipe_labels, "SLURM_TEMPLATE", getParams(panpipe_labels,"SLURM_GROUP_TEMPLATE"))
                 if participant_label:
                     updateParams(panpipe_labels,"GROUP_PARTICIPANTS_LABEL",participant_label)
                     updateParams(panpipe_labels,"GROUP_PARTICIPANTS_XNAT_PROJECT",project_list)
+                    updateParams(panpipe_labels,"GROUP_PARTICIPANTS_XNAT_SHARED_PROJECT",shared_project_list)
                     updateParams(panpipe_labels,"GROUP_SESSION_LABEL",session_list)
                 else:
                     updateParams(panpipe_labels,"GROUP_PARTICIPANTS_LABEL","*")
                     updateParams(panpipe_labels,"GROUP_PARTICIPANTS_XNAT_PROJECT","*")
+                    updateParams(panpipe_labels,"GROUP_PARTICIPANTS_XNAT_SHARED_PROJECT","*")
                     updateParams(panpipe_labels,"GROUP_SESSION_LABEL","*")
 
             else:
                 updateParams(panpipe_labels, "SLURM_TEMPLATE", getParams(panpipe_labels,"SLURM_PARTICIPANT_TEMPLATE"))
 
             if analysis_node == "gpu":
                 updateParams(panpipe_labels, "SLURM_HEADER", getParams(panpipe_labels,"SLURM_GPU_HEADER"))
@@ -317,32 +320,33 @@
             
             try:
                 procs = getProcNums(panpipe_labels)
 
                 if analysis_level == "participant":
                     # run serially if procs < 2
                     if procs > 1:
-                        multiproc_zip = zip(participant_list,project_list,session_list)
+                        multiproc_zip = zip(participant_list,project_list,shared_project_list,session_list)
                         parrunSingleSubject=partial(runSingleSubject, pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level=analysis_level)
                         with mp.Pool(procs) as pool:
                             completedlist = pool.starmap(parrunSingleSubject,multiproc_zip)
                             pool.close()
                             pool.join()
                     else:
                         for part_count in range(len(participant_list)):
                             if session_list:
                                 session_label= session_list[part_count]
                             else:
                                 session_label=None
-                            runSingleSubject(participant_list[part_count], project_list[part_count],session_label,pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level=analysis_level)
+                            runSingleSubject(participant_list[part_count], project_list[part_count], shared_project_list[part_count],session_label,pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level=analysis_level)
                 else:
                     updateParams(panpipe_labels,"GROUP_PARTICIPANTS_LABEL",participant_list)
                     updateParams(panpipe_labels,"GROUP_PARTICIPANTS_XNAT_PROJECT",project_list)
                     updateParams(panpipe_labels,"GROUP_SESSION_LABEL",session_list)
-                    runGroupSubjects(participant_list, project_list,session_list,pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level=analysis_level)
+                    updateParams(panpipe_labels,"GROUP_PARTICIPANTS_XNAT_SHARED_PROJECT",shared_project_list)
+                    runGroupSubjects(participant_list, project_list,shared_project_list,session_list,pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level=analysis_level)
 
 
             except Exception as ex:
                 LOGGER.info(f"problems running pipeline {pipeline}. Details: {ex}")
  
         else:
             LOGGER.info(f"processing environment {processing_environment} not currently supported. Options are {PROCESSING_OPTIONS}.")
```

### Comparing `panpipelines-0.9.7/src/panpipelines/single_subject.py` & `panpipelines-0.9.8/src/panpipelines/single_subject.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,28 @@
 from panpipelines import Factory
 
 LOGGER = logger_setup("panpipelines.single_subject", logging.DEBUG)
 logger_addstdout(LOGGER, logging.INFO)
 
 panFactory = Factory.getPANFactory()
 
-def runSingleSubject(participant_label, xnat_project, session_label, pipeline, pipeline_class, pipeline_outdir, panpipe_labels,bids_dir,cred_user,cred_password, execution_json,analysis_level="participant",panlabel=None):
+def runSingleSubject(participant_label, xnat_project, xnat_shared_project, session_label, pipeline, pipeline_class, pipeline_outdir, panpipe_labels,bids_dir,cred_user,cred_password, execution_json,analysis_level="participant",panlabel=None):
 
     pipeline_start = datetime.datetime.now()
     LOGGER.info("---------------------------------------------------------------------------------")
-    LOGGER.info(f"Single Subject Processing for {participant_label} started at: {str(pipeline_start)}")
+    LOGGER.info(f"Single Subject Processing for sub-{participant_label},ses-{session_label} started at: {str(pipeline_start)}")
+    LOGGER.info(f"Participant Label: {participant_label}")
+    LOGGER.info(f"Participant Session: {session_label}")
+    LOGGER.info(f"Participant Project: {xnat_project}")
+    LOGGER.info(f"Participant Shared Project: {xnat_shared_project}")
     LOGGER.info("---------------------------------------------------------------------------------")
 
     panpipe_labels = updateParams(panpipe_labels,"PARTICIPANT_LABEL",participant_label)
     panpipe_labels = updateParams(panpipe_labels,"PARTICIPANT_XNAT_PROJECT",xnat_project)
+    panpipe_labels = updateParams(panpipe_labels,"PARTICIPANT_XNAT_SHARED_PROJECT",xnat_shared_project)
     panpipe_labels = updateParams(panpipe_labels,"PARTICIPANT_SESSION",session_label)
 
     if not panlabel:
         # get parent directory
         panlabel=os.path.basename(os.path.dirname(pipeline_outdir))
 
     pipeline_outdir=os.path.join(pipeline_outdir,xnat_project)
@@ -160,19 +165,23 @@
         if not sessions_file:
             df = pd.read_table(participants_file,sep="\t")
         else:
             df = pd.read_table(sessions_file,sep="\t")
         if participant_index <= len(df):
             participant_label = drop_sub(df['bids_participant_id'].iloc[participant_index - 1])
             xnat_project = df['project'].iloc[participant_index - 1]
+            if 'shared_projects' in df.columns:
+                xnat_shared_project = df['shared_projects'].iloc[participant_index - 1]
+            else:
+                xnat_shared_project =""
             if sessions_file:
                 session_label = drop_ses(df['bids_session_id'].iloc[participant_index - 1])
             else:
                 session_label=None
-            runSingleSubject(participant_label,xnat_project,session_label, pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level="participant")
+            runSingleSubject(participant_label,xnat_project,xnat_shared_project,session_label, pipeline=pipeline, pipeline_class=pipeline_class, pipeline_outdir=pipeline_outdir, panpipe_labels=panpipe_labels,bids_dir=bids_dir,cred_user=cred_user,cred_password=cred_password, execution_json=execution_json,analysis_level="participant")
 
 
         else:
             print("Problem: ARRAY_INDEX {} greater than length of participants file {}".format(participant_index,participants_file))
     else:
         print("{} used as ARRAY_INDEX but not defined in os.environs".format(ARRAY_INDEX))
```

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/antstransform.py` & `panpipelines-0.9.8/src/panpipelines/nodes/antstransform.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/aslprep.py` & `panpipelines-0.9.8/src/panpipelines/nodes/aslprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/atlascreate.py` & `panpipelines-0.9.8/src/panpipelines/nodes/atlascreate.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/basil.py` & `panpipelines-0.9.8/src/panpipelines/nodes/basil.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,14 +97,16 @@
 
 
 def process_fmriprep_fieldmap(fmriprep_fieldmap_dir,layout, asljson , asl_acq, basil_dict, labels_dict, command_base, work_dir,fmap_mode="fmriprep"):
     IFLOGGER.info(f"Preparing fieldmap from {fmap_mode} for use in SDC.")
     fmap = getGlob(os.path.join(fmriprep_fieldmap_dir,"*desc-preproc_fieldmap.nii.gz"))
     fmaprads = newfile(work_dir,assocfile=fmap,intwix="desc-rads")
     fmapjson = getGlob(os.path.join(fmriprep_fieldmap_dir,"*desc-preproc_fieldmap.json"))
+    xnat_project = getParams(labels_dict,"PARTICIPANT_XNAT_PROJECT")
+    xnat_shared_project = getParams(labels_dict,"PARTICIPANT_XNAT_SHARED_PROJECT")
 
     IFLOGGER.info(f"Fieldmap located at {fmap}")
     fmapdict={}
     if fmapjson:
         with open(fmapjson,"r") as infile:
             fmapdict=json.load(infile)
 
@@ -169,25 +171,47 @@
         runCommand(evaluated_command,IFLOGGER)
 
         basil_dict = updateParams(basil_dict,FMAPMAG,fmapmag)
         basil_dict = updateParams(basil_dict,FMAPMAGBRAIN,fmapmag_brain)
 
     if os.path.exists(fmapmag_brain):
         echospacing = None
-        ECHOSPACING_DICT= getParams(labels_dict,"ASL_ECHOSPACING")
-        if ECHOSPACING_DICT is not None and isinstance(ECHOSPACING_DICT, dict):
-            if asl_acq in ECHOSPACING_DICT.keys():
-                echospacing = ECHOSPACING_DICT[asl_acq]
-
-        basil_dict = updateParams(basil_dict,ECHOSPACING,echospacing)
-        if echospacing:
-            IFLOGGER.info(f"Echospacing {echospacing} obtained from config file.")   
-        else:
-            IFLOGGER.error(f"Echospacing not defined. Fieldmap correction will not work.") 
-            raise ValueError("<ASL_ECHOSPACING> not defined in config file for fieldmap processing.") 
+
+        if "EffectiveEchoSpacing" in asljson.keys():
+            echospacing = asljson["EffectiveEchoSpacing"]
+            IFLOGGER.info(f"Echospacing {echospacing} obtained from BIDS metadata") 
+        
+        if not echospacing:
+            IFLOGGER.info(f"Echospacing not found in BIDS metadata. Attempting to retrieve from config file.") 
+            ECHOSPACING_DICT= getParams(labels_dict,"ASL_ECHOSPACING")
+            if ECHOSPACING_DICT is not None and isinstance(ECHOSPACING_DICT, dict):
+                if asl_acq in ECHOSPACING_DICT.keys():
+                    if ECHOSPACING_DICT[asl_acq] is not None and isinstance(ECHOSPACING_DICT[asl_acq], dict):
+                        if xnat_project in ECHOSPACING_DICT[asl_acq].keys():
+                            echospacing = ECHOSPACING_DICT[asl_acq][xnat_project]
+
+                        elif xnat_shared_project in ECHOSPACING_DICT[asl_acq].keys():
+                            echospacing = ECHOSPACING_DICT[asl_acq][xnat_shared_project]
+                        
+                        elif "default" in ECHOSPACING_DICT[asl_acq].keys():
+                            echospacing = ECHOSPACING_DICT[asl_acq]["default"]
+
+                        else:
+                            IFLOGGER.info(f"ASL_ECHOSPACING Dictionary keys {ECHOSPACING_DICT[asl_acq].keys()} not valid") 
+
+                    else:
+                        echospacing = ECHOSPACING_DICT[asl_acq]
+     
+            if echospacing:
+                IFLOGGER.info(f"Echospacing {echospacing} obtained from config file.")   
+            else:
+                IFLOGGER.error(f"Echospacing not defined. Fieldmap correction will not work.") 
+                raise ValueError("<ASL_ECHOSPACING> not defined in config file for fieldmap processing.")
+
+        basil_dict = updateParams(basil_dict,ECHOSPACING,echospacing) 
         pedir_ijk = asljson["PhaseEncodingDirection"]
         IFLOGGER.info(f"PE Direction of ASL is {pedir_ijk}")   
         pedir_fsl = pedir_ijk.replace('j-','-y').replace('j','y').replace('i-','-x').replace('i','x').replace('k-','-z').replace('k','z')
         IFLOGGER.info(f"PE Direction of ASL converted to {pedir_fsl} for BASIL.")    
         basil_dict = updateParams(basil_dict,PEDIR,pedir_fsl)
```

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/collate_csv_group.py` & `panpipelines-0.9.8/src/panpipelines/nodes/collate_csv_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/collate_csv_single.py` & `panpipelines-0.9.8/src/panpipelines/nodes/collate_csv_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/dummy.py` & `panpipelines-0.9.8/src/panpipelines/nodes/dummy.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/fmriprep.py` & `panpipelines-0.9.8/src/panpipelines/nodes/fmriprep.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/freesurfer.py` & `panpipelines-0.9.8/src/panpipelines/nodes/freesurfer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/fslanat.py` & `panpipelines-0.9.8/src/panpipelines/nodes/fslanat.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/glm_randomize_group.py` & `panpipelines-0.9.8/src/panpipelines/nodes/glm_randomize_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/lst.py` & `panpipelines-0.9.8/src/panpipelines/nodes/lst.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/noddi.py` & `panpipelines-0.9.8/src/panpipelines/nodes/noddi.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/parse_textdata.py` & `panpipelines-0.9.8/src/panpipelines/nodes/parse_textdata.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/preproc.py` & `panpipelines-0.9.8/src/panpipelines/nodes/preproc.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,24 +38,16 @@
 # simulate strel('disk',3)
 disc3 = np.ones((5,5,5))
 
 streldict={
     "disc5" : disc5,
     "disc3" : disc3,
     "disc2" : disc2
-
 }
 
-FRAC_INT_THRESH="0.7000000000000002"
-VERT_GRAD="0"
-RINGTHRESH = 0.15
-STRELCLOSE = disc3
-PHASESHIFT=14
-PHASEAXIS=1
-
 
 IFLOGGER=nlogging.getLogger('nipype.interface')
 
 def returnCandidates(p0,p1,p2):
     arrayList=[]
     max_x = np.max(np.array([p0[0],p1[0],p2[0]]))
     max_y = np.max(np.array([p0[1],p1[1],p2[1]]))
@@ -76,15 +68,200 @@
     n = np.cross(p1-p0,p2-p0)/npl.norm(np.cross(p1-p0,p2-p0))
     d = np.dot(n,p-p1)
     if np.abs(d) < tol:
         return True
     else:
         return False
 
-def derive_asl_artefact_v1(aslfile,aslfile_brain,aslfile_brain_mask,workdir,outputdir,RINGTHRESH=RINGTHRESH,STRELCLOSE=STRELCLOSE,PHASESHIFT=PHASESHIFT,PHASEAXIS=PHASEAXIS):
+def derive_asl_artefact_v2(asl_acq,labels_dict,command_base,participant_label,participant_session,artefact_outputdir,PHASESHIFT=12,PHASEAXIS=1,ALLOWOVERLAP=False,CLOSE_DISC=1,DILATE_DISC=2):
+    
+    transform_list =  getParams(labels_dict,'TRANSFORM_MAT')
+    transform_ref =  getParams(labels_dict,'TRANSFORM_REF')
+    PHASESHIFT_lookup = getParams(labels_dict,'PHASESHIFT')
+    if PHASESHIFT_lookup:
+        if isinstance(PHASESHIFT_lookup,dict):
+            if asl_acq in PHASESHIFT_lookup.keys():
+                PHASESHIFT=int(PHASESHIFT_lookup[asl_acq])
+        else:
+            PHASESHIFT = int(PHASESHIFT_lookup)
+    if getParams(labels_dict,'PHASEAXIS'):
+        PHASEAXIS = int(getParams(labels_dict,'PHASEAXIS'))
+    if getParams(labels_dict,'CLOSE_DISC'):
+        CLOSE_DISC = int(getParams(labels_dict,'CLOSE_DISC'))
+    if getParams(labels_dict,'DILATE_DISC'):
+        DILATE_DISC = int(getParams(labels_dict,'DILATE_DISC'))
+    if getParams(labels_dict,'ALLOWOVERLAP'):
+        ALLOWOVERLAP = isTrue(getParams(labels_dict,'ALLOWOVERLAP'))
+
+    cwd = os.getcwd()
+    output_dir=cwd
+
+    work_dir=os.path.join(output_dir,"preproc_workdir")
+    if not os.path.exists(work_dir):
+        os.makedirs(work_dir)
+
+    labels_dict = updateParams(labels_dict,"CWD",cwd)
+
+    # set up dwi to process just the specific dwi session
+    subject = f"sub-{participant_label}"
+    if participant_session:
+        session = f"ses-{participant_session}"
+    else:
+        session=""
+
+    if not artefact_outputdir:
+        artefact_outputdir = os.path.join(output_dir,"asl_artefact", subject,session)
+    else:
+        artefact_outputdir = os.path.join(artefact_outputdir,"asl_artefact", subject,session)
+
+    if not os.path.exists(artefact_outputdir):
+        os.makedirs(artefact_outputdir, exist_ok=True)
+
+
+    subjects_dir = getParams(labels_dict,'SUBJECTS_DIR')
+    outer_skull=os.path.join(subjects_dir,subject,'bem','outer_skull.surf')
+
+    params =  f" --subject {subject}" \
+            f" --subjects_dir {subjects_dir}" 
+    PREPROC_CONTAINER_TO_USE = getParams(labels_dict,"PREPROC_CONTAINER_TO_USE")
+    if PREPROC_CONTAINER_TO_USE:
+        panscript = pancontainer_script.pancontainer_panscript(labels_dict,params=params,command=f"python {mne_make_surfaces.__file__}",container_img=PREPROC_CONTAINER_TO_USE)
+    else: 
+        panscript = pancontainer_script.pancontainer_panscript(labels_dict,params=params,command=f"python {mne_make_surfaces.__file__}")
+    panscript.run()
+    os.chdir(output_dir)
+
+    rr_mm_outer_skull,tris_outer_skull = mne.read_surface(outer_skull)
+
+    orig_file=f"{subjects_dir}/{subject}/mri/T1.mgz"
+    origimg = nibabel.load(orig_file)
+    Torig = origimg.header.get_vox2ras_tkr()
+    origimg_dtype = origimg.header.get_data_dtype()
+    origimg_shape = origimg.shape
+    outer_skull_vol = np.zeros((origimg_shape),dtype=origimg_dtype)
+    inv_Torig = npl.inv(Torig)
+
+    for rr in rr_mm_outer_skull:
+        vox = apply_affine(inv_Torig, rr)
+        vox_ind = tuple(np.round(vox).astype(int))
+        outer_skull_vol[vox_ind] = 255
+
+    for tri in tris_outer_skull:
+        p0 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[0]])).astype(int)
+        p1 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[1]])).astype(int)
+        p2 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[2]])).astype(int)
+        valid_vox = returnCandidates(p0,p1,p2)
+        for vox in valid_vox:
+            vox_ind = tuple(vox.astype(int))
+            outer_skull_vol[vox_ind] = 255
+    outer_skull_img = nibabel.Nifti1Image(outer_skull_vol,origimg.affine,origimg.header)
+    outer_skull_img_file=os.path.join(work_dir,f"{subject}_{session}_outer_skull.nii.gz")
+    nibabel.save(outer_skull_img,outer_skull_img_file) 
+
+    outer_skull_aslspace_file = None
+    if transform_list and transform_ref:
+        results = antstransform_proc(labels_dict, outer_skull_img_file,transform_list, transform_ref)
+        outer_skull_aslspace_file = results['out_file']     
+
+    outer_skull_aslspace_bin=newfile(work_dir,outer_skull_aslspace_file,suffix="bin")
+    command = f"{command_base} fslmaths {outer_skull_aslspace_file} -abs -bin {outer_skull_aslspace_bin}"
+    evaluated_command=substitute_labels(command, labels_dict)
+    results = runCommand(evaluated_command,IFLOGGER)
+
+    outskull_aslspace_img=nibabel.load(outer_skull_aslspace_bin)
+    outskull_aslspace_data = outskull_aslspace_img.get_fdata()
+    outskull_aslspace_file  = outer_skull_aslspace_bin
+
+    if DILATE_DISC > 0:
+        disc = np.ones((DILATE_DISC,DILATE_DISC,DILATE_DISC))
+        outskull_aslspace_data_dilation = ndimage.binary_dilation(outskull_aslspace_data, structure=disc).astype(np.int16)
+        outskull_aslspace_data_dilation_file=newfile(work_dir,outskull_aslspace_file,suffix=f"dilation-disc-{DILATE_DISC}")
+        outskull_aslspace_data_dilation_img = nibabel.Nifti1Image(outskull_aslspace_data_dilation,outskull_aslspace_img.affine,outskull_aslspace_img.header)
+        nibabel.save(outskull_aslspace_data_dilation_img,outskull_aslspace_data_dilation_file)
+        outskull_aslspace_file = outskull_aslspace_data_dilation_file
+        outskull_aslspace_data = outskull_aslspace_data_dilation
+    
+    if CLOSE_DISC > 0:
+        disc = np.ones((CLOSE_DISC,CLOSE_DISC,CLOSE_DISC))
+        outskull_aslspace_data_close = ndimage.binary_closing(outskull_aslspace_data, structure=disc).astype(np.int16)
+        outskull_aslspace_data_close_file=newfile(work_dir,outskull_aslspace_file,suffix=f"close-disc-{CLOSE_DISC}")
+        outskull_aslspace_data_close_img = nibabel.Nifti1Image(outskull_aslspace_data_close,outskull_aslspace_img.affine,outskull_aslspace_img.header)
+        nibabel.save(outskull_aslspace_data_close_img,outskull_aslspace_data_close_file)
+        outskull_aslspace_file = outskull_aslspace_data_close_file
+        outskull_aslspace_data = outskull_aslspace_data_close
+
+    out_dims = outskull_aslspace_data.shape
+    if PHASESHIFT < 0:
+        PHASESHIFT_CALC = out_dims[PHASEAXIS] + PHASESHIFT
+        OVSTART=PHASESHIFT_CALC
+        OVEND=-1
+    else:
+        PHASESHIFT_CALC = PHASESHIFT
+        OVSTART=0
+        OVEND=PHASESHIFT
+
+    outer_skull_shift=newfile(work_dir,outskull_aslspace_file,suffix="shift")
+    data_shifted = np.roll(outskull_aslspace_data,PHASESHIFT_CALC,PHASEAXIS)
+    if not ALLOWOVERLAP:
+        if PHASEAXIS==0:
+            data_shifted[OVSTART:OVEND,:,:]=0
+        elif PHASEAXIS==1:
+            data_shifted[:,OVSTART:OVEND,:]=0
+        elif PHASEAXIS==2:
+            data_shifted[:,:,OVSTART:OVEND]=0
+        else:
+            print(f"phase axis {PHASEAXIS} not valid. Allowing overlap of mask")     
+    shifted_img = nibabel.Nifti1Image(data_shifted,outskull_aslspace_img.affine,outskull_aslspace_img.header)
+    nibabel.save(shifted_img,outer_skull_shift)
+    outskull_aslspace_file = outer_skull_shift
+    outskull_aslspace_data = data_shifted
+
+    outer_skull_shift_final = newfile(artefact_outputdir,assocfile=f"{subject}_{session}_asl_chemical_shift_artefact.nii.gz")
+    shutil.copyfile(outer_skull_shift,outer_skull_shift_final)  
+
+
+def derive_asl_artefact_v1(asl_acq,labels_dict,command_base,aslfile,aslfile_brain,aslfile_brain_mask,workdir,outputdir,RINGTHRESH=0.15,STRELCLOSE=disc3,PHASESHIFT=12,PHASEAXIS=1,FRAC_INT_THRESH="0.7000000000000002",VERT_GRAD="0"):
+
+    FRAC_INT_THRESH_lookup= getParams(labels_dict,'FRAC_INT_THRESH')
+    if FRAC_INT_THRESH_lookup:
+        FRAC_INT_THRESH = FRAC_INT_THRESH_lookup
+
+    VERT_GRAD_lookup=getParams(labels_dict,'VERT_GRAD')
+    if VERT_GRAD_lookup:
+        VERT_GRAD = VERT_GRAD_lookup
+
+    RINGTHRESH_lookup=getParams(labels_dict,'RINGTHRESH')
+    if RINGTHRESH_lookup:
+        RINGTHRESH = np.float64(RINGTHRESH_lookup)
+
+    STRELCLOSE_lookup=getParams(labels_dict,'STRELCLOSE')
+    if STRELCLOSE_lookup and STRELCLOSE_lookup in streldict.keys():
+        STRELCLOSE = streldict[STRELCLOSE_lookup]
+
+    PHASESHIFT_lookup = getParams(labels_dict,'PHASESHIFT')
+    if PHASESHIFT_lookup:
+        if isinstance(PHASESHIFT_lookup,dict):
+            if asl_acq in PHASESHIFT_lookup.keys():
+                PHASESHIFT=int(PHASESHIFT_lookup[asl_acq])
+        else:
+            PHASESHIFT = int(PHASESHIFT_lookup)
+    if getParams(labels_dict,'PHASEAXIS'):
+        PHASEAXIS = int(getParams(labels_dict,'PHASEAXIS'))
+
+    params=f" {aslfile}" \
+        f" {aslfile_brain}" \
+        " -R" \
+        f" -f {FRAC_INT_THRESH}" \
+        f" -g {VERT_GRAD}" \
+        " -m -s"
+
+    command=f"{command_base} bet"\
+        " "+params
+    evaluated_command=substitute_labels(command, labels_dict)
+    results = runCommand(evaluated_command,IFLOGGER)
 
     data1 = nibabel.load(aslfile).get_fdata()
     data1 = data1[:,:,:,0]
     data2img = nibabel.load(aslfile_brain)
     data2 = data2img.get_fdata()
     data3img = nibabel.load(aslfile_brain_mask)
     data3 = data3img.get_fdata()
@@ -146,164 +323,56 @@
     evaluated_command=substitute_labels(command, labels_dict)
     results = runCommand(evaluated_command,IFLOGGER)
 
     # set up dwi to process just the specific dwi session
     participant_label = getParams(labels_dict,'PARTICIPANT_LABEL')
     subject = f"sub-{participant_label}"
     participant_session = getParams(labels_dict,'PARTICIPANT_SESSION')
-    session = f"sub-{participant_session}"
+    session = f"ses-{participant_session}"
     preproc_version = getParams(labels_dict,'PREPROC_VERSION')
     if preproc_version:
         VERSION_TO_RUN = preproc_version
     else:
         VERSION_TO_RUN = "2"
 
     # calculate asl artefact for acq-prod
     layout = BIDSLayout(bids_dir)
-    asl=layout.get(subject=participant_label,session=participant_session,acquisition="prod",suffix='asl', extension='nii.gz')
+    asl=layout.get(subject=participant_label,session=participant_session,suffix='asl', extension='nii.gz')
 
     if len(asl) > 0:
+        asl_bidsfile=asl[0]
+        asl_entities = asl_bidsfile.get_entities()
+        if "acquisition" in asl_entities.keys():
+            asl_acq = "acq-" + asl_entities["acquisition"]
+        else:
+            asl_acq = get_bidstag("acq",asl_bidsfile.filename)
+
+        if not asl_acq:
+            asl_acq = "default"
 
         artefact_outputdir = getParams(labels_dict,'DERIVATIVES_DIR')
         if not artefact_outputdir:
             artefact_outputdir = os.path.join(output_dir,"asl_artefact", subject,session)
         else:
             artefact_outputdir = os.path.join(artefact_outputdir,"asl_artefact", subject,session)
 
         if not os.path.exists(artefact_outputdir):
             os.makedirs(artefact_outputdir, exist_ok=True)
 
         if VERSION_TO_RUN == "2":
-            subjects_dir = getParams(labels_dict,'SUBJECTS_DIR')
-            params =  f" --subject {subject}" \
-                    f" --subjects_dir {subjects_dir}" 
-            PREPROC_CONTAINER_TO_USE = getParams(labels_dict,"PREPROC_CONTAINER_TO_USE")
-            if PREPROC_CONTAINER_TO_USE:
-                panscript = pancontainer_script.pancontainer_panscript(labels_dict,params=params,command=f"python {mne_make_surfaces.__file__}",container_img=PREPROC_CONTAINER_TO_USE)
-            else: 
-                panscript = pancontainer_script.pancontainer_panscript(labels_dict,params=params,command=f"python {mne_make_surfaces.__file__}")
-            panscript.run()
-
-            os.chdir(output_dir)
-
-            outer_skull=os.path.join(subjects_dir,subject,'bem','outer_skull.surf')
-            rr_mm_outer_skull,tris_outer_skull = mne.read_surface(outer_skull)
-
-            orig_file=f"{subjects_dir}/{subject}/mri/T1.mgz"
-            origimg = nibabel.load(orig_file)
-            Torig = origimg.header.get_vox2ras_tkr()
-            origimg_dtype = origimg.header.get_data_dtype()
-            origimg_shape = origimg.shape
-            outer_skull_vol = np.zeros((origimg_shape),dtype=origimg_dtype)
-            inv_Torig = npl.inv(Torig)
-
-            for rr in rr_mm_outer_skull:
-                vox = apply_affine(inv_Torig, rr)
-                vox_ind = tuple(np.round(vox).astype(int))
-                outer_skull_vol[vox_ind] = 1
-
-            for tri in tris_outer_skull:
-                p0 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[0]])).astype(int)
-                p1 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[1]])).astype(int)
-                p2 = np.round(apply_affine(inv_Torig,rr_mm_outer_skull[tri[2]])).astype(int)
-                valid_vox = returnCandidates(p0,p1,p2)
-                for vox in valid_vox:
-                    vox_ind = tuple(vox.astype(int))
-                    outer_skull_vol[vox_ind] = 1
-            outer_skull_img = nibabel.Nifti1Image(outer_skull_vol,origimg.affine,origimg.header)
-            outer_skull_img_file=os.path.join(work_dir,f"{subject}_{session}_outer_skull.nii.gz")
-            nibabel.save(outer_skull_img,outer_skull_img_file) 
-
-            transform_list =  getParams(labels_dict,'TRANSFORM_MAT')
-            transform_ref =  getParams(labels_dict,'TRANSFORM_REF')
-            outer_skull_aslspace_file = None
-            if transform_list and transform_ref:
-                results = antstransform_proc(labels_dict, outer_skull_img_file,transform_list, transform_ref)
-                outer_skull_aslspace_file = results['out_file']     
-
-            outer_skull_aslspace_bin=newfile(work_dir,outer_skull_aslspace_file,suffix="bin")
-            command = f"{command_base} fslmaths {outer_skull_aslspace_file} -bin {outer_skull_aslspace_bin}"
-            evaluated_command=substitute_labels(command, labels_dict)
-            results = runCommand(evaluated_command,IFLOGGER)
-
-            outskull_aslspace_img=nibabel.load(outer_skull_aslspace_bin)
-            outskull_aslspace_data = outskull_aslspace_img.get_fdata()
-            outskull_aslspace_data_close = ndimage.binary_closing(outskull_aslspace_data, structure=disc5).astype(np.int16)
-            outskull_aslspace_data_close_file=newfile(work_dir,outer_skull_aslspace_bin,suffix="close-disc-5")
-            outskull_aslspace_data_close_img = nibabel.Nifti1Image(outskull_aslspace_data_close,outskull_aslspace_img.affine,outskull_aslspace_img.header)
-            nibabel.save(outskull_aslspace_data_close_img,outskull_aslspace_data_close_file)  
-
-            outer_skull_shift=newfile(work_dir,outskull_aslspace_data_close_file,suffix="shift")
-            data_shifted = np.roll(outskull_aslspace_data_close,PHASESHIFT,1)
-            data_shifted[:,0:PHASESHIFT,:]=0
-            shifted_img = nibabel.Nifti1Image(data_shifted,outskull_aslspace_img.affine,outskull_aslspace_img.header)
-            nibabel.save(shifted_img,outer_skull_shift)
-
-            outer_skull_shift_final = newfile(artefact_outputdir,assocfile=f"{subject}_{session}_asl_chemical_shift_artefact.nii.gz")
-            shutil.copyfile(outer_skull_shift,outer_skull_shift_final)  
-
+            derive_asl_artefact_v2(asl_acq,labels_dict,command_base, participant_label,participant_session,artefact_outputdir)
         else:
-            FRAC_INT_THRESH_lookup= getParams(labels_dict,'FRAC_INT_THRESH')
-            if FRAC_INT_THRESH_lookup:
-                FRAC_INT_THRESH = FRAC_INT_THRESH_lookup
-
-            VERT_GRAD_lookup=getParams(labels_dict,'VERT_GRAD')
-            if VERT_GRAD_lookup:
-                VERT_GRAD = VERT_GRAD_lookup
-
-            RINGTHRESH_lookup=getParams(labels_dict,'RINGTHRESH')
-            if RINGTHRESH_lookup:
-                RINGTHRESH = np.float64(RINGTHRESH_lookup)
-
-            STRELCLOSE_lookup=getParams(labels_dict,'STRELCLOSE')
-            if STRELCLOSE_lookup and STRELCLOSE_lookup in streldict.keys():
-                STRELCLOSE = streldict[STRELCLOSE_lookup]
-
-            asl_bidsfile=asl[0]
-            asl_file=asl_bidsfile.path
-            asl_file_brain = newfile(work_dir,assocfile=asl_file,suffix="brain")
-            asl_file_brain_mask = newfile(work_dir,assocfile=asl_file_brain,suffix="mask")
-
-            params=f" {asl_file}" \
-                f" {asl_file_brain}" \
-                " -R" \
-                f" -f {FRAC_INT_THRESH}" \
-                f" -g {VERT_GRAD}" \
-                " -m -s"
-
-            command=f"{command_base} bet"\
-                " "+params
-            evaluated_command=substitute_labels(command, labels_dict)
-            results = runCommand(evaluated_command,IFLOGGER)
-
-            derive_asl_artefact_v1(asl_file,asl_file_brain,asl_file_brain_mask,work_dir,artefact_outputdir,RINGTHRESH=RINGTHRESH,STRELCLOSE=STRELCLOSE)
-
-            asl_entities = asl_bidsfile.get_entities()
             m0_entities = asl_entities.copy()
             m0_entities["suffix"]="m0scan"
             m0  = layout.get(return_type='file', invalid_filters='allow', **m0_entities)
             if len(m0) > 0:
                 m0_file=m0[0]
                 m0_file_brain = newfile(work_dir,assocfile=m0_file,suffix="brain")
                 m0_file_brain_mask = newfile(work_dir,assocfile=m0_file_brain,suffix="mask")
-
-                params=f" {m0_file}" \
-                    f" {m0_file_brain}" \
-                    " -R" \
-                    f" -f {FRAC_INT_THRESH}" \
-                    f" -g {VERT_GRAD}" \
-                    " -m -s"
-
-                command=f"{command_base} bet"\
-                    " "+params
-                evaluated_command=substitute_labels(command, labels_dict)
-                results = runCommand(evaluated_command,IFLOGGER)
-
-                derive_asl_artefact_v1(m0_file,m0_file_brain,m0_file_brain_mask,work_dir,artefact_outputdir,RINGTHRESH=RINGTHRESH,STRELCLOSE=STRELCLOSE)
-
+                derive_asl_artefact_v1(asl_acq,labels_dict, command_base, m0_file,m0_file_brain,m0_file_brain_mask,work_dir,artefact_outputdir)
 
     return {
         "output_dir":output_dir
     }
```

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/qsiprep.py` & `panpipelines-0.9.8/src/panpipelines/nodes/qsiprep.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,35 @@
 
     command_base, container = getContainer(labels_dict,nodename="qsiprep", SPECIFIC="QSIPREP_CONTAINER",LOGGER=IFLOGGER)
     IFLOGGER.info("Checking the qsiprep version:")
     command = f"{command_base} --version"
     evaluated_command=substitute_labels(command, labels_dict)
     results = runCommand(evaluated_command,IFLOGGER)
 
+    # set up dwi to process just the specific dwi session
+    participant_label = getParams(labels_dict,'PARTICIPANT_LABEL')
+    participant_session = getParams(labels_dict,'PARTICIPANT_SESSION')
+
     eddy_config = getParams(labels_dict,'EDDY_CONFIG')
     eddy_json=""
     if eddy_config:
         if os.path.exists(eddy_config):
             with open(eddy_config, 'r') as infile:
                 eddy_json = json.load(infile)
         if eddy_json:
             IFLOGGER.info(f"eddy params provided in file {eddy_config} and contents are:")
             IFLOGGER.info(f"{eddy_json}")
 
+    eddy_update = getParams(labels_dict,'EDDY_CONFIG_UPDATE')
 
-    # set up dwi to process just the specific dwi session
-    participant_label = getParams(labels_dict,'PARTICIPANT_LABEL')
-    participant_session = getParams(labels_dict,'PARTICIPANT_SESSION')
+    if eddy_json and eddy_update and isinstance(eddy_update,dict):
+        for itemkey,itemvalue in eddy_update.items():
+            eddy_json[itemkey] = substitute_labels(itemvalue,labels_dict)
+        eddy_config = newfile(cwd,eddy_config,prefix=f"sub-{participant_label}_ses-{participant_session}")
+        export_labels(eddy_json, eddy_config)
 
     # This is for 1 specific scenario - we will terminate early if field map is missing
     layout = BIDSLayout(bids_dir)
     epi = layout.get(subject=participant_label, session=participant_session, suffix="epi",extension=".nii.gz") 
     if not epi:
         IFLOGGER.warn(f"Fieldmap not found for subject {participant_label} and session {participant_session}. terminating script early.")
         sys.exit(1)
@@ -63,15 +70,15 @@
     qsiprep_dict = updateParams(qsiprep_dict,"--participant_label","<PARTICIPANT_LABEL>")
     qsiprep_dict = updateParams(qsiprep_dict,"--separate-all-dwis",IS_PRESENT)
     qsiprep_dict = updateParams(qsiprep_dict,"--bids-filter-file",bids_filter_file)
     qsiprep_dict = updateParams(qsiprep_dict,"--skip-bids-validation",IS_PRESENT)
     qsiprep_dict = updateParams(qsiprep_dict,"--hmc-model" ,"eddy")
     qsiprep_dict = updateParams(qsiprep_dict,"--unringing-method" ,"rpg")
     qsiprep_dict = updateParams(qsiprep_dict,"--b1-biascorrect-stage","none")
-    qsiprep_dict = updateParams(qsiprep_dict,"--eddy-config" ,"<EDDY_CONFIG>")
+    qsiprep_dict = updateParams(qsiprep_dict,"--eddy-config" ,eddy_config)
     qsiprep_dict = updateParams(qsiprep_dict,"--mem_mb","<BIDSAPP_MEMORY>")
     qsiprep_dict = updateParams(qsiprep_dict,"--nthreads","<BIDSAPP_THREADS>")
     qsiprep_dict = updateParams(qsiprep_dict,"--fs-license-file","<FSLICENSE>")
     qsiprep_dict = updateParams(qsiprep_dict,"--write-graph",IS_PRESENT)
     qsiprep_dict = updateParams(qsiprep_dict,"--output-resolution","<OUTPUT_RES>")
     qsiprep_dict = updateParams(qsiprep_dict,"-w","<CWD>/qsiprep_work")
```

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/roi_extract.py` & `panpipelines-0.9.8/src/panpipelines/nodes/roi_extract.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/roi_mean_group.py` & `panpipelines-0.9.8/src/panpipelines/nodes/roi_mean_group.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/roi_mean_single.py` & `panpipelines-0.9.8/src/panpipelines/nodes/roi_mean_single.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/nodes/tensor.py` & `panpipelines-0.9.8/src/panpipelines/nodes/tensor.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/aslprep_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/aslprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/basil_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/basil_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/collatecsv_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/collatecsv_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/collatecsvgroup_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/dummy_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/dummy_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/fmriprep_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/fmriprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/freesurfer_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/freesurfer_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/lst_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/lst_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/noddi_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/noddi_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/preproc_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/preproc_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/qsiprep_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/qsiprep_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/roiextract_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/roiextract_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/tensor_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/tensor_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/textmeasures_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/textmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/pipelines/volmeasures_panpipeline.py` & `panpipelines-0.9.8/src/panpipelines/pipelines/volmeasures_panpipeline.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/scripts/aslprep_panscript.py` & `panpipelines-0.9.8/src/panpipelines/scripts/aslprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/scripts/fmriprep_panscript.py` & `panpipelines-0.9.8/src/panpipelines/scripts/fmriprep_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/scripts/mne_make_surfaces.py` & `panpipelines-0.9.8/src/panpipelines/scripts/mne_make_surfaces.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/scripts/pancontainer_panscript.py` & `panpipelines-0.9.8/src/panpipelines/scripts/pancontainer_panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/scripts/panscript.py` & `panpipelines-0.9.8/src/panpipelines/scripts/panscript.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/scripts/sdcflows_fieldmap.py` & `panpipelines-0.9.8/src/panpipelines/scripts/sdcflows_fieldmap.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/utils/transformer.py` & `panpipelines-0.9.8/src/panpipelines/utils/transformer.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/utils/util_functions.py` & `panpipelines-0.9.8/src/panpipelines/utils/util_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 def drop_sub(value):
     return re.sub(r"^sub-", "", str(value))
 
 def drop_ses(value):
     return re.sub(r"^ses-", "", str(value))
 
 def isTrue(arg):
-    return arg is not None and (arg == 'Y' or arg == 'y' or arg == '1' or arg == 'True' or arg == 'true')
+    return arg is not None and (arg == 'Y' or arg == 'y' or arg == '1' or arg == 'True' or arg == 'true' or arg == True)
 
 def getParams(pardict, key, update=True):
     if key is not None and pardict is not None:
         if key in pardict:
             if update:
                 updateParams(pardict,key,pardict[key])
                 return pardict[key] 
@@ -700,14 +700,15 @@
         participants = df["bids_participant_id"].tolist()
 
     # process exclusions
     participants = list(set(participants).difference(set(subject_exclusions)))
 
     # sessions are defined and so we will use this as priority
     project_list=[]
+    shared_project_list=[]
     participant_list=[]
     sessions_list=[]
     if sessions_file is not None and session_labels:
         sessions_df = pd.read_table(sessions_file,sep="\t")
         # participants and sessions are defined
         if participants is not None and len(participants) > 0:
             for participant in participants:
@@ -715,37 +716,46 @@
                     search_df = sessions_df[(sessions_df["bids_participant_id"]=="sub-" + drop_sub(participant))]
                     ses=[drop_ses(ses) for ses in list(search_df.bids_session_id.values)]
                     sessions_list.extend(ses)
                     sub=[drop_sub(sub) for sub in list(search_df.bids_participant_id.values)]
                     participant_list.extend(sub)
                     proj=[proj for proj in list(search_df.project.values)]
                     project_list.extend(proj)
+                    if 'shared_projects' in df.columns:
+                        shared_proj=[shared_proj for shared_proj in list(search_df.shared_projects.values)]
+                        shared_project_list.extend(shared_proj)
                 else: 
                     for session_label in session_labels:
                         search_df = sessions_df[(sessions_df["bids_participant_id"]=="sub-" + drop_sub(participant)) & (sessions_df["bids_session_id"].str.contains(session_label))]
                         if search_df.empty:
                             UTLOGGER.info(f"No values found for {participant} and {session_label} in {sessions_file}")
                         else:
                             ses=[drop_ses(ses) for ses in list(search_df.bids_session_id.values)]
                             sessions_list.extend(ses)
                             sub=[drop_sub(sub) for sub in list(search_df.bids_participant_id.values)]
                             participant_list.extend(sub)
                             proj=[proj for proj in list(search_df.project.values)]
                             project_list.extend(proj)
+                            if 'shared_projects' in df.columns:
+                                shared_proj=[shared_proj for shared_proj in list(search_df.shared_projects.values)]
+                                shared_project_list.extend(shared_proj)
         else:
             UTLOGGER.info(f"Cannot process pipelines. No participants have been specified")
     else:
         if participants is not None and len(participants) > 0:
             for participant in participants:
                 project_list.append(str(df[df["bids_participant_id"]==participant].project.values[0]))
+                if 'shared_projects' in df.columns:
+                    shared_project_list.append(str(df[df["bids_participant_id"]==participant].shared_projects.values[0]))
+                                
             sessions_list=[None for proj in project_list]
         else:
             UTLOGGER.info(f"Cannot process pipelines. No participants have been specified")
 
-    return  [ participant_list, project_list,sessions_list ]
+    return  [ participant_list, project_list, sessions_list, shared_project_list ]
 
 
 def create_script(header,template,panpipe_labels, script_file, LOGGER=UTLOGGER):
     with open(header,"r") as infile:
         headerlines=infile.readlines()
 
     with open(template,"r") as infile:
@@ -1498,29 +1508,67 @@
 def initTemplateFlow(TEMPLATEFLOW_HOME):
     ref1=get_template_ref(TEMPLATEFLOW_HOME,"MNI152NLin2009cAsym",resolution=2,suffix="T1w",extension=[".nii.gz"])
     ref2=get_template_ref(TEMPLATEFLOW_HOME,"MNI152NLin6Asym",resolution=2,suffix="T1w",extension=[".nii.gz"])
     transform1 = get_template_ref(TEMPLATEFLOW_HOME,"MNI152NLin2009cAsym",suffix="xfm",extension=[".h5"])
     transform2 = get_template_ref(TEMPLATEFLOW_HOME,"MNI152NLin6Asym",suffix="xfm",extension=[".h5"])
     return [[ref1,transform1],[ref2,transform2]]
 
-def getBidsTSV(host,user,password,projects,targetfolder,outputdir,demographics=True):
+def getSharedProjects(connection, subjectLabel,origProjectID,sharedProjectIDs):
+    sharedProjects=[]
+    REVERSE=False
+
+    try:
+        apistring = f"/data/projects/{origProjectID}/subjects/{subjectLabel}/projects"
+        response = connection.get(apistring,query={"format":"json"})
+        responseJson = response.json()
+        if responseJson:
+            results = responseJson["ResultSet"]["Result"]
+            for result in results:
+                if "ID" in result.keys():
+                    for sharedProjectID in sharedProjectIDs:
+                        if result["ID"] == sharedProjectID:
+                            sharedProjects.append(sharedProjectID)
+
+    except Exception as e:
+        REVERSE=True
+
+    if REVERSE:
+            for sharedProjectID in sharedProjectIDs:
+                apistring = f"/data/projects/{sharedProjectID}/subjects/{subjectLabel}/projects"
+                try:
+                    response = connection.get(apistring,query={"format":"json"})
+                    responseJson = response.json()
+                    if responseJson:
+                        results = responseJson["ResultSet"]["Result"]
+                        for result in results:
+                            if "ID" in result.keys():
+                                    if result["ID"] == origProjectID:
+                                        sharedProjects.append(sharedProjectID)
+                except Exception as e:
+                    pass
+
+    sharedProjectString = ",".join(sharedProjects)
+    return sharedProjectString
+
+
+def getBidsTSV(host,user,password,projects,targetfolder,outputdir,demographics=True,shared_project_list=["001_HML","002_HML","003_HML","004_HML"]):
     import xnat
     from pydicom import dcmread
     import fnmatch
 
     if not os.path.isdir(outputdir):
         os.mkdir(outputdir)
 
     participantsTSV=os.path.join(outputdir,'participants.tsv')
     sessionsTSV=os.path.join(outputdir,'sessions.tsv')
 
-    participant_columns=['xnat_subject_id','xnat_subject_label','bids_participant_id','project','gender', 'age','scan_date','comments']
+    participant_columns=['xnat_subject_id','xnat_subject_label','bids_participant_id','project','shared_projects','gender', 'age','scan_date','comments']
     participant_data=[]
 
-    session_columns=['xnat_session_id','xnat_session_label','xnat_subject_id','xnat_subject_label','bids_participant_id','bids_session_id', 'project','gender', 'age','scan_date','comments']
+    session_columns=['xnat_session_id','xnat_session_label','xnat_subject_id','xnat_subject_label','bids_participant_id','bids_session_id', 'project', 'shared_projects','gender', 'age','scan_date','comments']
     session_data=[]
 
     scantest = os.path.join(outputdir,'scantest.dcm')
 
     with xnat.connect(server=host,user=user, password=password) as connection:
 
         if projects is None:
@@ -1543,14 +1591,15 @@
                     xnat_subject_label = ""
                     bids_participant_id = ""
                     bids_session_id = ""
                     gender = ""
                     age = ""
                     comments=""
                     scan_date=""
+                    shared_projects=""
 
 
                     # _MR_ hack - some reason 003_HML MR session not storing modality 
                     if experiment.modality == 'MR' or "_MR_" in experiment.label:
                         xnat_session_id = experiment.id
                         xnat_session_label = experiment.label
                         xnat_subject_id = experiment.subject.id
@@ -1589,21 +1638,23 @@
                                         scandate = datetime.datetime.strptime(scan_date,"%Y%m%d")
                                         if agedate is None or agedate == '':
                                             comments = "subject age missing; " + comments
                                         else:
                                             age=getAge(agedate,scandate)
                                         break
 
+                            shared_projects = getSharedProjects(connection, xnat_subject_label,project.id,shared_project_list)
+
                         except Exception as e:
                             message = 'problem parsing resource : %s.' % targetfolder
                             comments="missing bids files; " + comments
                             print(message)
                             print(str(e))
 
-                        session_data.append([xnat_session_id,xnat_session_label,xnat_subject_id,xnat_subject_label,bids_participant_id,bids_session_id, project.id, gender, age,scan_date,comments])
+                        session_data.append([xnat_session_id,xnat_session_label,xnat_subject_id,xnat_subject_label,bids_participant_id,bids_session_id, project.id, shared_projects,gender, age,scan_date,comments])
 
             except Exception as e:
                 message = 'problem parsing project :  %s.' % PROJ
                 print (message)
                 print(str(e))
 
         df = pd.DataFrame(session_data, columns=session_columns)
@@ -1734,20 +1785,20 @@
         container_prerun = getParams(labels_dict,f"{SPECIFIC}_PRERUN")
         container = getParams(labels_dict,f"{SPECIFIC}")
     else:
         container_run_options = None
         container_prerun = None
         container = None
 
-    if not container_run_options:
+    if container and not container_run_options:
         container_run_options = getParams(labels_dict,'CONTAINER_RUN_OPTIONS')
         if not container_run_options:
             container_run_options = ""
 
-    if not container_prerun:
+    if container and not container_prerun:
         container_prerun = getParams(labels_dict,'CONTAINER_PRERUN')
         if not container_prerun:
             container_prerun = ""
 
     if not container:
         container = getParams(labels_dict,'CONTAINER')
         if not container:
```

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/aslprep_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/aslprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/basil_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/basil_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/collatecsv_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/collatecsv_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/collatecsvgroup_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/collatecsvgroup_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/dummy_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/dummy_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/fmriprep_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/fmriprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/freesurfer_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/freesurfer_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/lst_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/lst_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/noddi_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/noddi_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/preproc_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/preproc_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/qsiprep_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/qsiprep_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/roiextract_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/roiextract_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/tensor_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/tensor_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/textmeasures_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/textmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/src/panpipelines/workflows/volmeasures_workflow.py` & `panpipelines-0.9.8/src/panpipelines/workflows/volmeasures_workflow.py`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/.gitignore` & `panpipelines-0.9.8/.gitignore`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/LICENSE` & `panpipelines-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/README.md` & `panpipelines-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/pyproject.toml` & `panpipelines-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panpipelines-0.9.7/PKG-INFO` & `panpipelines-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpipelines
-Version: 0.9.7
+Version: 0.9.8
 Summary: MRI Processing Pipelines for PAN Healthy Minds for Life Study
 Project-URL: Homepage, https://github.com/MRIresearch/PANpipelines
 Project-URL: Bug Tracker, https://github.com/MRIresearch/PANpipelines/issues
 Author-email: Chidi Ugonna <chidiugonna@arizona.edu>
 License: MIT License
         
         Copyright (c) 2023 MRIresearch
```

