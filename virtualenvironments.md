# Virtual Environments
Virtual environment is a tool that keeps the modules required by different projects in separate places.  

## Why is this important?
Your computer probably has several versions of python on it, and the python you are running is determined by your path.  Also, there are likely several versions of python's installation tool pip on your machine, and the pip you are using may not be installing the packages you want to the python you intended.  To avoid these complications, and to help contain only the modules you need for your specified project, you can use virtual environments.

## Get virtualenv
Install virtualenv to your default python:

  pip install virtualenv

## How to Make a Virtual Environment

  cd working_dir    # cd into your working directory
  virtualenv env    # this command creates your virtual 
		    # environment, complete with its 
		    # own version of python  

## How to Use your New Python
  source venv/bin/activate

## Use Your New pip to Install Your Requirements
For example 'pip install requests'.  We have in this repo a file that contains all of your requirements.  To install all of your requirements for this project type:
  
  pip install -r requirements.txt

## If in the future you add modules to your environment, you can list them in a requirements file.  The 'pip freeze' command will list your requirements along with the version.  To put All of Your Requirements into a Requirements file type:

  pip freeze > requirements.txt


For more information on virtual environments, and some tools to simplify them, see http://docs.python-guide.org/en/latest/dev/virtualenvs/
