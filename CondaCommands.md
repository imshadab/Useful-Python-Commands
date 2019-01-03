### 1. Check conda is installed and in your PATH

> conda -V

### 2. Check conda is up to date

> conda update conda

### 3. See a list of available python versions 

> conda search "^python$"

### 4. Create a virtual environment for your project

> conda create -n yourenvname python=x.x.x anaconda

Here you need to replace yourenvname with the name that you want to keep for your environment and x.x.x with the python version
you want to install, It will ask for your permission to download executable python and create other directories which you can 
simply proceed. A directory will be created with the same name that will contain all the files. Please run this command in the 
directory where you want to keep your project and create a virtual environment.

### Note: The virtual environment will be created in this directory:

> C:\Users\username\AppData\Local\Continuum\anaconda2\envs\yourenvname

__Here username is your computer's username__

The python file executable file is located in the same directory. There are two executable pythons:-
1. pythonw.exe
2. python.exe

If you're going to call a python script from some other process (say, from the command line), use pythonw.exe. Otherwise, your user will continuously see a cmd window launching the python process. It'll still run your script just the same, but it won't intrude on the user experience.

An example might be sending an email; python.exe will pop up a CLI window, send the email, then close the window. It'll appear as a quick flash, and can be considered somewhat annoying. pythonw.exe avoids this, but still sends the email.

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

