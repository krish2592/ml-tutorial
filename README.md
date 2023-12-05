# Initial Setup and environment for ML Project

## Setup python

### Go to official website and install python

https://www.python.org/downloads/ 

1. Windows:

     For windows download the executable file and run

2. Linux:

    For linux download the tar.xz file.

    Go to Downlaods. 

    For this project we are using Python-3.12.0.tar.xz. 

    You can download a specific version as per your operating system.

Open terminal and run the following command to install and verify

1. To extract
    ```tar -xf Python-3.12.0.tar.xz```

2. To configure
    ```cd Python-3.12.0```
    ```./configure```

3. To install
    ```sudo make install```

4. To verify
    ```python3 --version``` 


## Setup conda

Install conda as per your os distribution

    https://www.anaconda.com/download


After download run it

    bash ~/Downloads/Anaconda3-2023.09-0-Linux-x86_64.sh

Accept yes to user license agreement

source ~/.bashrc or re open the terminal to take effec

To activate wheather our base environment is activated auto on open or not

conda config --set auto_activate_base True

conda config --set auto_activate_base False


## Install code editor
   Download vscode as per your opersting system

   https://code.visualstudio.com/download

   Go to extension and enable plugin/extension Python by microsoft 


## Create a virtual environment

1. Create virtual environment using command

To create a environment at default loaction:

    conda create --name projectenv python=3.12 -y
    conda activate projectenv
    python --version

To create a environment at specific location:

   conda create --prefix /<path>/projectenv python=3.12 -y
   conda activate /<path>/projectenv

To create environment in current directory:

   conda create --prefix projectenv python=3.12 -y
   conda activate /<path>/projectenv

To deactivate:

  conda deactivate

2. Create virtual environment using script/yaml file

This will be added later

    conda env create -f config-env.yml
    conda activate projectenv

