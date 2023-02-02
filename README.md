# fsRL5k
Implementation of a 5k vertex fsRL surface for vertex wise connectomes generation

# path to surfaces and spheres
/data/mica3/BIDS_MICs/conte69-10k/surface/deformed*
fs_LR-deformed_to-fsaverage.R.sphere.5k_fs_LR.surf.gii
regular.sphere.5k.surf.gii

## New naming scheme
| Original                           | micapipe                             |
|------------------------------------|--------------------------------------|
| deformed_fsLR_5k.L.surf.gii        | fsLR_5k_hemi-L.surf.gii              |
| deformed_fsLR_5k.R.surf.gii        | fsLR_5k_hemi-R.surf.gii              |
| deformed_fsLR.L.sphere.5k.surf.gii | fsLR_5k_hemi-L_space-sphere.surf.gii |
| deformed_fsLR.R.sphere.5k.surf.gii | fsLR_5k_hemi-R_space-sphere.surf.gii |
| deformed_mask_5k_lh.func.gii       | fsLR_5k_hemi-L_label-mask.func.gii   |
| deformed_mask_5k_rh.func.gii       | fsLR_5k_hemi-R_label-mask.func.gii   |

# Generate ROIs from surface: script ``rerun_mrisconvert.sh`
line 70-77
surf2roy.py

# Mapping feature to surface
workflow_wb_command.sh
/data/mica3/BIDS_MICs/conte69-10k/code/worklog_allsteps.sh
