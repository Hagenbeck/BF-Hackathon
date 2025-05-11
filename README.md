# This repository is for the BadenovaNetze Challenge

## Reproduction
#### If you want to do all the data preprocessing as we did:
1. Install the dependencies (lower in the readme)
3. Load original_data into another folder called Hackathon-Daten next to the working directory and unzip all of them.
4. Run the alkis_join Notebook to merge the Gemarkungs-Files (the output directory is set correctly)
5. Run the solar_join Notebook to merge the Solarpotenzial-Files
6. Save the "Strom-Einspeiser-Export 1.csv" as UTF
7. Perform a spatial join on following layers with gebaeudebauwerke as base-layer: gebaeudebauwerke.shp, Strom-Einspeiser-Export 1.csv, solarpotenzial.shp, nexiga_all.shp (in our case the solar_potenzial data had to be repaired with qgis)
8. Run the PU_learner on the joined_data
9. Now you can visualize the houses that had all data in a GIS application

#### If you don't want to do the data processing:
Approach the team to get the merged file (only if you are allowed to get the data)

### To install the dependencies with the anaconda prompt do the following:
- Find bf-hack.yml
- If you have an already deprecated version of the environment you can override it with `conda env update --name hack --file <path/to/bf-hack.yaml> --prune`
- execute following in the anaconda prompt `conda env create -f <path/to/environment-specification.yaml>`
  
### If you want to add a dependency do the following:
- Install dependency: `conda install -c conda-forge <dependency>`
- Export env `conda env export > bf-hack.yaml`
- Commit env
