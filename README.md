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

## Download and save WorldClim data in /data folder

Donwload Bioclim data

    wget -P ~/checkouts/sdm-toolbox/data https://geodata.ucdavis.edu/climate/worldclim/2_1/base/wc2.1_10m_bio.zip
    unzip wc2.1_10m_bio.zip -d ~/checkouts/sdm-toolbox/data

Download Topography data

    wget -P ~/checkouts/sdm-toolbox/data https://geodata.ucdavis.edu/climate/worldclim/2_1/base/wc2.1_10m_elev.zip
    unzip wc2.1_10m_elev.zip -d ~/checkouts/sdm-toolbox/data

Download Planted Forest East Asia data

    mkdir ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia
    wget https://figshare.com/ndownloader/files/41222433 -O ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/PlantedForestEastAsia.shp
    wget https://figshare.com/ndownloader/files/41222436 -O ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/PlantedForestEastAsia.shx
    wget https://figshare.com/ndownloader/files/41222439 -O ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/PlantedForestEastAsia.prj
    wget https://figshare.com/ndownloader/files/41222430 -O ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/PlantedForestEastAsia.dbf
    cd ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/
    zip planted-forest-east-asia.zip *
