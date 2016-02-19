#Welcome to Introduction to Python 2016!

The materials collected in this repository are a collaborative effort between Caroline Harbitz (https://github.com/cterp) and myself (https://github.com/ginaschmalzle).  The purpose -- learn Python!  Why? 'Cause it's cool.

This repository contains all the information you need to participate in the workshop.  It contains interactive python notebooks and tutorials, as well as some practice assignments.  

##Directions to download this repository:

You can download this repository to your local machine by clicking the 'Download ZIP' button on this webpage.  Or, if you want to impress your friends you can do it this way:

1. Open a terminal
2. Make sure you have git installed.  You can check by typing ```which git``` at the terminal prompt.  If a path appears continue to step 4.
3. Install git (https://git-scm.com/book/en/v1/Getting-Started-Installing-Git). If you are on a mac, we recommend using homebrew (http://brew.sh/) to install git.
4. In your working directory type:
    ```git clone https://github.com/ginaschmalzle/git-your-python-booty.git```

Interested in using git?

This is a simple explanation of some of the most common commands:

http://rogerdudler.github.io/git-guide/


# Running the Code
You will need to download some additional modules for this workshop.  

### pip
The easiest python package management system to use is pip. If you do not have pip, you can install pip using easy_install. Here are the steps:

1. Check to see if you have pip. If a path is returned you have pip; continue to the next session.

    ```which pip```


2. Check to see if you have easy_install:

    ```which easy_install```

If a path is returned type:

    easy_install pip

### Install other requirements and launch Jupyter
Once you have pip installed move to your cloned directory and type:

    pip install -r requirements.txt

To start your session type:

    jupyter notebook



# Extra Credit

## Virtual Environments
Virtual environment is a tool that keeps the modules required by different projects in separate places.  

### Why is this important?
Your computer probably has several versions of python on it, and the python you are running is determined by your path.  Also, there are likely several versions of python's installation tool pip on your machine, and the pip you are using may not be installing the packages you want to the python you intended.  To avoid these complications, and to help contain only the modules you need for your specified project, you can use virtual environments.

### Get virtualenv
In your working directory, install virtualenv to your default python:

    cd working_dir    # cd into your working directory
    pip install virtualenv

### How to Make a Virtual Environment
The following command creates a virtual environment:

    virtualenv env    # this command creates your virtual environment, complete with its own version of python  

### How to Use your New Python
This command tells your computer to use the version of python you just created:

    source env/bin/activate

### Use Your New pip to Install Your Requirements
Now that you're pointed to the new python environment, install all of your requirements for this project:

    pip install -r requirements.txt

### Updating Your Requirements
If in the future you add or remove modules to your virtual environment, you can list them in a requirements file.  The 'pip freeze' command will list your requirements along with the version.  To put All of Your Requirements into a Requirements file type:

    pip freeze > requirements.txt

For more information on virtual environments, and some tools to simplify them, see http://docs.python-guide.org/en/latest/dev/virtualenvs/
