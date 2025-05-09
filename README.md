# This repository is for the BadenovaNetze Challenge

### To install the dependencies with the anaconda prompt do the following:
- Find bf-hack.yml
- If you have an already deprecated version of the environment delete the old version with `conda env remove --name hack`
- execute following in the anaconda prompt `conda env create -f <path/to/environment-specification.yaml>`
  
### If you want to add a dependency do the following:
- Install dependency: `conda install -c conda-forge <dependency>`
- Export env `conda env export > bf-hack.yaml`
- Commit env