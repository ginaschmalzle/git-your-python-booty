#Welcome to Python Bootcamp 2015!

The materials collected in this repository are a collaborative effort between Caroline Harbitz (https://github.com/cterp) and myself (https://github.com/ginaschmalzle).  The purpose -- learn python!  Why? Cause it's cool.

This repository contains all the information you need to participate in the bootcamp.  It contains interactive python notebooks and tutorials, as well as some practice assignments.  

Directions to install:

You can download this repository to your local machine by clicking the 'Clone in Desktop' button on this webpage.  Or if you are savvy and want to impress your friends you can do it by:

1. Open a terminal
2. Make sure you have git installed.  You can check by typing 'which git' at the terminal prompt.  If a path appears continue to step 4.
3. Install git.   Go to your terminal and type:

    brew update

    brew install git
4. In your working directory type:
    git clone https://github.com/ginaschmalzle/git-your-python-booty.git


Interested in using git?

This is a simple explaination of some of the most common commands:

http://rogerdudler.github.io/git-guide/


# Running the Code
We recommend that you use virtual environments for your projects.  This helps keep a record of which modules you will need for each project, as well as a clean way of identifying which python you are using.  Below is a description of Virtual Environments and directions for using them for this project.

## Virtual Environments
Virtual environment is a tool that keeps the modules required by different projects in separate places.  

### Why is this important?
Your computer probably has several versions of python on it, and the python you are running is determined by your path.  Also, there are likely several versions of python's installation tool pip on your machine, and the pip you are using may not be installing the packages you want to the python you intended.  To avoid these complications, and to help contain only the modules you need for your specified project, you can use virtual environments.

### Get virtualenv
Install virtualenv to your default python:

  pip install virtualenv

### How to Make a Virtual Environment

  cd working_dir    # cd into your working directory
  virtualenv env    # this command creates your virtual
		    # environment, complete with its
		    # own version of python  

### How to Use your New Python
  source venv/bin/activate

### Use Your New pip to Install Your Requirements
For example 'pip install requests'.  We have in this repo a file that contains all of your requirements.  To install all of your requirements for this project type:

  pip install -r requirements.txt

### Updating Your Requirements
If in the future you add or remove modules to your virtual environment, you can list them in a requirements file.  The 'pip freeze' command will list your requirements along with the version.  To put All of Your Requirements into a Requirements file type:

  pip freeze > requirements.txt


For more information on virtual environments, and some tools to simplify them, see http://docs.python-guide.org/en/latest/dev/virtualenvs/
