# Through-Terminal-Via-Brew

<br>

## What this repository is about?
This repository is about how to install libraries and applications on OS X through terminal using Homebrew package manager. So why Homebrew? Homebrew is an application that installs libraries or application for you with just a command(s). An application might/usually come with other dependencies which also needs to be downloaded manually by you, well if you Homebrew that won't be necessary anymore. Homebrew will figure out and install the dependencies for you. At some point if do not need an application(s) or library(s) anymore, you can just fire up the terminal and run a single command to uninstall and homebrew will uninstall it and/or delete any files associated with it. [This is the link to Homebrew's website](https://brew.sh/) if one wants to know more about it.

<br>

## *To install any libraries or applications you must have the right priveligies or be the super user of your computer.*

<br>

## Before installing *Homebrew*, *Xcode* must be installed.
Run **`$ which g++`** to see if ***Xcode*** installed or not. If not, run **`$ xcode-select --install`** to install ***Xcode***.

Once ***Xcode*** is installed successfully, ***Homebrew*** can be installed using the command below -  
**`$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`**

To verify if Homebrew has been successfully installed or not check the current version by the command below -  
**`$ brew -v`**

<br>

## ***Brew*** commands for installing Libraries and Applications
  * [install ***Google Chrome*** via ***brew***](#google-chrome)
  * [install ***Firefox*** via ***brew***](#firefox)
  

## <a name="google-chrome">Insatlling Google Chrome using brew</a>
To install the Google Chrome on your **OS X** just run the command below. ***Brew*** will download the latest version of   Google Chrome and will place it in under ***Applications***.  
**`$ brew cask install google-chrome`**


## <a name="firefox">Insatlling Firefox using brew</a>
To install the Firefox on your **OS X** just run the command below. ***Brew*** will download the latest version of Firefox  
and will place it in under ***Applications***.  
**`$ brew cask install firefox`**


