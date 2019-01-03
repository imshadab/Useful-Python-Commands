### 1. Check conda is installed and in your PATH

> conda -V

### 2. Check conda is up to date

> conda update conda

### 3. See a list of available python versions 

> conda search "^python$"

### 4. Create a virtual environment for your project

conda create -n yourenvname python=x.x.x anaconda

Here you need to replace yourenvname with the name that you want to keep for your environment and x.x.x with the python version
you want to install, It will ask for your permission to download executable python and create other directories which you can 
simply proceed. A directory will be created with the same name that will contain all the files. Please run this command in the 
directory where you want to keep your project and create a virtual environment.

### 5. Activate your virtual environment.

> conda activate yourenvname 

### 6. Deactivate your virtual environment

> conda deactivate

### 7. See a list of all environments

> conda info -e

### 8. Install additional Python packages to a virtual environment

> conda install -n yourenvname [package]

### 9. Delete a virtual environment that is no longer needed

> conda remove -n yourenvname -all
