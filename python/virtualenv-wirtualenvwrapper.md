#How to to activate venv

install pip
`sudo apt-get install python3-pip`

install virtualenv (by using pip or pip3)
`pip install virtualenv`

install virtualenvwrapper

create environment variable for venv
`export WORKON_HOME=~/envs`

Add the following lines to ~/.bashrc:

`export PROJECT_HOME=$HOME/repos`

`VIRTUALENVWRAPPER_PYTHON='/usr/bin/python3' # This needs to be placed before the virtualenvwrapper command`

`source /usr/local/bin/virtualenvwrapper.sh`

##Common commands

Create virtualenv
`mkvirtualenv virtualenv_name` 

Activate/switch to a virtualenv
`workon virtualenv_name`

`deactivate virtualenv_nam`

##Projects

Attach existing code with virtual env
1. Create and activate virtual env
2. Move to project directory
3. run setvirtualenvproject to attach project directory with virtualenv

Create new virtual env and project

`mkproject`

