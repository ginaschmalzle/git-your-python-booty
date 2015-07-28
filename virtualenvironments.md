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
For example 'pip install requests'.  If a requirements.txt file exists for your project, you can type 'pip install -r requirements.txt

## Put All of Your Requirements into a Requirements file
  pip freeze > requirements.txt


For more information on virtual environments, and some tools to simplify them, see http://docs.python-guide.org/en/latest/dev/virtualenvs/
