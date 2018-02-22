# Python Setup

This document descibes common steps that you will require to install the required software/packages required to quickly setup a python project and start developing. 

#### Open a Terminal

You will be using a termminal program like (terminal or iterm) for doing most of the setup required. If you have never used a terminal program ordo not know how to use the terminal and setup environment variables, take a few minutes and get familiar with the terminal program. Here are a few articles to help you with that. 

https://lifehacker.com/5633909/who-needs-a-mouse-learn-to-use-the-command-line-for-almost-anything

http://osxdaily.com/2015/07/28/set-enviornment-variables-mac-os-x/

#### Check python version installed on the system

 On Mac OS X, the default version of python is 2.x (like 2.7.10). To check the currently installed version, type `python —version` in the terminal shell prompt. If python is already installed, you should see a valid version like `Python 2.7.10`. If python is not installed, download python from https://www.python.org/downloads and install it. 

#### Install git

You will most likely want to keep the source code for your project under a source code control system like **git**. Again, Mac OS X probably already have a version of **git** installed. Check if **git** installed and install it if required. 

On Mac OS X **git** will be available if **Xcode** and **Apple command line tools** are installed. Type `git` from the terminal prompt. If **git** is installed you should see **git** command like options and help message. If **XCode** and **Apple command line tools** are not installed, you will be prompted to install **Xcode**. Click **Install** to install Xcode and Apple command like tools. When this completes **git** should be available in the system.

#### Install HomeBrew

Some packages may require [HomeBrew](https://brew.sh/). If HomeBrew is not installed, install it.

```
$ which brew
```

If HomeBrew is not installed (if `which brew` command returns an error like `brew not found`), install it. Follow the instruction in https://brew.sh/

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Follow the prompts to install. May ask for password. If Home brew is installed (if `which brew` command returns a valid path like `/usr/local/bin/brew`), update it. 

```
brew update
```

#### Install pip

Install `pip` if it not already installed. `pip` is the official python package manager. 

Check if pip is already installed. 

```
which pip
```

If `which pip` command returns an error like `pip not found`, install it. Follow the instructions in https://pip.pypa.io/en/stable/installing/ to install `pip`. If `pip` is already installed (if the `which pip` command returns a valid path like `/usr/local/bin/pip`), skip this step.

#### Install pipenv 

Install `pipenv` if not already installed. [pipenv](https://pypi.python.org/pypi/pipenv)  is the officially recommended python packaging tool. It automatically creates and manages a virtualenv for your projects, as well as adds/removes packages from your `Pipfile` as you install/uninstall packages.