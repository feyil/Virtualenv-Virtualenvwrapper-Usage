## Virtualenv Virtualenvwrapper Usage

Inludes Description of How to Use Virtualenv and Virtualenvwrapper with Python

### Installation

* Using pip install virtualenv and virtualenvwrapper to the system.

```shell
$ sudo pip install virtualenv virtualenvwrapper
```

* Create a **.virtualenvs** folder in your root

```shell
$ cd ~
$ mkdir .virtualenvs
```

* Using vim add the following lines to your **.bashrc**

```shell
# virtualenv and virtualenvwrapper
export WORKON_HOME=$HOME/.virtualenvs
export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3
source /usr/local/bin/virtualenvwrapper.sh
```

* Restart the bash session. Alternativly run

```shell
source ~/.bashrc
```

### Virtualenvwrapper Usage

* Creating a virtualenv **mkvirtualenv**. It creates and start the env with [ENV_NAME]

```shell
$ mkvirtualenv [ENV_NAME] -p python[VERSION]
([ENV_NAME]) $ 
```

* Deactivating an environment

```shell
([ENV_NAME]) $ deactivate
$
```

* Activating an environment

```shell
$ workon [ENV_NAME]
([ENV_NAME]) $
```

* Deleting  an environment

```shell
$ rmvirtualenv [ENV_NAME]
```

* Showing available virtualenvwrapper commands:

```shell
$ virtualenvwrapper
  add2virtualenv: add directory to the import path

  allvirtualenv: run a command in all virtualenvs

  cdproject: change directory to the active project

  cdsitepackages: change to the site-packages directory

  cdvirtualenv: change to the $VIRTUAL_ENV directory

  cpvirtualenv: duplicate the named virtualenv to make a new one

  lssitepackages: list contents of the site-packages directory

  lsvirtualenv: list virtualenvs

  mkproject: create a new project directory and its associated virtualenv

  mktmpenv: create a temporary virtualenv

  mkvirtualenv: Create a new virtualenv in $WORKON_HOME

  rmvirtualenv: Remove a virtualenv

  setvirtualenvproject: associate a project directory with a virtualenv

  showvirtualenv: show details of a single virtualenv

  toggleglobalsitepackages: turn access to global site-packages on/off

  virtualenvwrapper: show this help message

  wipeenv: remove all packages installed in the current virtualenv

  workon: list or change working virtualenvs
```

### References

[how-to-install-opencv-4-on-ubuntu](https://www.pyimagesearch.com/2018/08/15/how-to-install-opencv-4-on-ubuntu/)

[configuring-python-environment-with-virtualenvwrapper](https://medium.com/the-andela-way/configuring-python-environment-with-virtualenvwrapper-8745c2895745)