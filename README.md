#  Installing conda

Conda is powerful package manager and helps install, runs packages and their dependencies.A conda envirnoment contains a specific collection of packages that is installed such as BWA, and other bioinformatics tools.

# STEPS/Installation of conda on linux

Go to the webiste:https://www.anaconda.com/products/distribution

wget https://repo.anaconda.com/archive/Anaconda3-2022.10-Linux-x86_64.sh
 
bash Anaconda3-2022.10-Linux-x86_64.sh
 > Follow the instruction to review the lincese
 
 conda --v
 
 conda config --show channels
 
 conda config --add channels conda-forge
 
 conda config --add channels bioconda
 
 conda config --show channels
 
 # Create a Conda envirnoment commands;
 
 Conda env list
  #this envirnoment will be empty so you can create env and activate the envirnoment to use all the packages and tools installed
 
 conda create -n Name of the Env
 
 conda activate Name of the Env
 
 conda deactivate 
 
 Note:Conda env has to be activated in order to use tools installed in the envirnoment
 
 # Installing bioinformatics tools such as BWA, bowtie, minimap2 can be easily installed by these command line.
 
 conda install -c bioconda bwa 
 
 conda install -c bioconda minimap2

 conda install -c bioconda bowtie2

