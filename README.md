# SDM-Toolbox
A toolbox for specie distribution modelling in Maxent

## Create a conda environment for this project

    conda env create --file conda-environment.yml
    conda activate sdm-toolbox

## Clone this repository

In order to keep track of your github repositories on your computer, it is recommended to store them in a `checkouts` folder in your `home` folder.

    mkdir ~/checkouts
    cd ~/checkouts
    git clone https://github.com/janjaapmeijer/sdm-toolbox sdm-toolbox

## Download and save WorldClim data

**Bioclim dataset**

    wget -P ~/checkouts/sdm-toolbox/data https://geodata.ucdavis.edu/climate/worldclim/2_1/base/wc2.1_10m_bio.zip
    unzip wc2.1_10m_bio.zip -d ~/checkouts/sdm-toolbox/data

**Topography dataset**

    wget -P ~/checkouts/sdm-toolbox/data https://geodata.ucdavis.edu/climate/worldclim/2_1/base/wc2.1_10m_elev.zip
    unzip wc2.1_10m_elev.zip -d ~/checkouts/sdm-toolbox/data

## Download additional data

**Land Cover/ Forest Type dataset**

[Copernicus Dynamic Land Cover](https://land.copernicus.eu/en/products/global-dynamic-land-cover)

    wget https://zenodo.org/records/3939050/files/PROBAV_LC100_global_v3.0.1_2019-nrt_Forest-Type-layer_EPSG-4326.tif -P ~/checkouts/sdm-toolbox/data/species/land-cover/


**Planted Forest East Asia data dataset from Abbasi et al. 2023**

    mkdir ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia
    wget https://figshare.com/ndownloader/files/41222433 -O ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/PlantedForestEastAsia.shp
    wget https://figshare.com/ndownloader/files/41222436 -O ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/PlantedForestEastAsia.shx
    wget https://figshare.com/ndownloader/files/41222439 -O ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/PlantedForestEastAsia.prj
    wget https://figshare.com/ndownloader/files/41222430 -O ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/PlantedForestEastAsia.dbf
    cd ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/
    zip planted-forest-east-asia.zip *
