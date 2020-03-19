# Conda Environment for Python 3.6 and Biopython

Guide for building a Conda environment for Python 3.6 and Biopython

## Summary - Installation 
1. Clone Repository 
2. Install Conda if not already in environment
3. Create conda environment

## Test Environment
1. Activate conda environment - `conda activate py36_biopython`
2. Deactivate conda environment - `conda deactivate`

## Clone this code using GIT

### Install git for Debian systems using the following command (if necessary)
```
sudo apt update
sudo apt install git
```

##Installation directions 
These instructions install the code into your home path. Change the instructions if appropriate. 

### Clone the code from repository
```
cd ~
git clone https://github.com/jiangweiyao/py36_biopython.git
```

### Install Miniconda (if no Conda is install on system). 
You can run the prepackaged script install_miniconda.sh to install into your home directory (recommended) by using the following command
```
. ~/py36_biopython/install_miniconda.sh
```

Detailed instruction on the the Miniconda website if anything goes wrong:
https://conda.io/projects/conda/en/latest/user-guide/install/linux.html

### Clone the environment. Need to do once.

We use conda to create an environment (that we can activate and deactivate) to install our dependent software and resolve their dependencies. This environment is called "py36_biopython". The following command assumes your environment file is in your home path. Modify as appropriate.

```
conda env create -f ~/py36_biopython/py36_biopython.yml
```

The command to generate the environment originally is in the included `py36_biopython.txt` file. 

## Run the code.

Activating your environment makes the software you installed in that environment available for use. You will see "(py36_biopython)" in front bash after activation.
```
conda activate py36_biopython
```

When you are finished running the workflow, exit out of your environment by running `conda deactivate`. Deactivating your environment exits out of your current environment and protects it from being modified by other programs. You can build as many environments as you want and enter and exit out of them. Each environment is separate from each other to prevent version or dependency clashes. The author recommands using Conda/Bioconda to manage your dependencies.


