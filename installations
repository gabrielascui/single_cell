## walkthrough installation of required software and R packages

############## Software installation ############## 

## get miniconda3
wget https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda.sh

bash miniconda.sh

## add to .bashrc
export PATH=/home/gascui/miniconda3/bin:$PATH

# make sure to have correct python and conda
which conda
which python

## install R

conda install -c r r

## install Jupyter Labs

conda install -c conda-forge jupyterlab

## run jupyter labs and create jupyter notebook 

jupyter lab --no-browser --port 2323 &

## install R kernel for jupyter

conda install -c r r-irkernel

## check everything
which conda
which R
which python
which jupyter

############## Seurat 3.0 installation ############## 

## install Seurat 3.0 ##

install.packages('devtools')
devtools::install_github(repo = 'satijalab/seurat', ref = 'release/3.0')

### If you have a problem with Seurat dependencies to 'hdf5r', this is a go-around solution. Worked for me. 

install.packages("remotes")
remotes::install_github("UCSF-TI/fake-hdf5r")
devtools::install_github(repo = 'satijalab/seurat', ref = 'release/3.0')
library('Seurat')

### More to come.
