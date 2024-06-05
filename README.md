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
    wget https://figshare.com/ndownloader/files/41222433 -O PlantedForestEastAsia.shp -P ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/
    wget https://figshare.com/ndownloader/files/41222436 -O PlantedForestEastAsia.shx -P ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/
    wget https://figshare.com/ndownloader/files/41222439 -O PlantedForestEastAsia.prj -P ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/
    wget https://figshare.com/ndownloader/files/41222430 -O PlantedForestEastAsia.shp -P ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/
    wget https://figshare.com/ndownloader/articles/21774725/versions/3 -O planted-forest-east-asia.zip -P ~/checkouts/sdm-toolbox/data/species/planted-forest-east-asia/
