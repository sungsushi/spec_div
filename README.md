# Repository for ``Diverse and specialized connectivity facilitates multimodal roles in annotated connectomes'' by Moon & Ahnert. 

## About:
- This is the repo accompanying the preprint Moon et al., 2025, containing all scripts needed to generate the results. 

## Installation:
- Run ```pip install requirements.txt``` in your ```python``` environment of choice.
- Then run Jupyter notebooks to do analysis and generate figures into the ```figures``` folder. 

## Contents:
### ```src``` 
- ```\module\convect``` CONVECT, a CONnectivity VECTorisation analysis tool for annotated networks. 
- ```ipynb``` Jupyter notebooks are in ```src```
    - ```01_vec_ent_nb.ipynb``` includes code for running the connectivity vectorisation, entropy calculations and the specialization-diversity calculations, then plotting distributions. We process these into connectivity vectors and specialization-diversity dataframes which are saved in generated ```data/*/processed``` subfolders. **Creates figure 2 in Moon et al., 2025.** 
        - In addition to figures in the publication, we have plotly iframes for reference in ```figures/distributions_vis```. 
    - ```02_null_models_nb.ipynb``` includes null models of the specialization-diversity entropic vector euclidean pairwise distances for cell types, serial homologues and left-right pairs. **Creates figure 3 in Moon et al., 2025.**
    - ```ZZ_supplementary.ipynb``` includes analysis for supplementary figures. 

###  ```data```

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.15052465.svg)](https://doi.org/10.5281/zenodo.15052465)

Please download from the Zenodo link above and save into the repository directory.
- ```celegans``` is a folder for celegans 
    - ```/materials/072022_anatomical_class.csv``` is metadata from Ripoll-Sanchez et al., _Neuron_ (2023).
    - ```/original/white_1986_whole.csv``` is an edge list from [nemanode](www.nemanode.org) (Witvliet et al., _Nature_ (2021), based on Varshney et al., _PLOS Computational Biology_ (2011) and White et al., _Philos Trans R Soc Lond B Biol Sci_ (1986)).
    - ```Cell_lists_herm.csv```,  ```Cell_lists_sexshared.csv```,  ```pharynx_ctypes.csv``` are neuron classifications from Cook et al., _Nature_ (2019). These ```csv```s are separated out from from the ```xlsx``` file ```SI 4 Cell lists.xlsx```, available from [wormwiring](https://wormwiring.org/pages/adjacency.html). 
- ```20241119_dm_data``` is the _Drosophila_ VNC data pull of the Male Adult Nerve Cord (MANC) connectome and metadata pulled on 19/11/2024, Cheong et al., _eLife_ (2024), available from [neuprint](https://neuprint.janelia.org/). 
    - ```manc_edges_20241119.csv``` is the edge list. 
    - ```manc_meta_20241119.csv``` is the metadata.





