# :hammer_and_wrench: Through-Terminal-Via-Brew :computer:

<br>

## :man_technologist: What this repository is about?
This repository is about how to install libraries and applications on OS X through terminal using Homebrew package manager. So why Homebrew? Homebrew is an application that installs libraries or application for you with just a command(s). An application might/usually come with other dependencies which also needs to be downloaded manually by you, well if you Homebrew that won't be necessary anymore. Homebrew will figure out and install the dependencies for you. At some point if do not need an application(s) or library(s) anymore, you can just fire up the terminal and run a single command to uninstall and homebrew will uninstall it and/or delete any files associated with it. [This is the link to Homebrew's website](https://brew.sh/) if one wants to know more about it.

<br>

## :stop_sign: *To install any libraries or applications you must have the right priveligies or be the super user of your computer.*

<br>

## :construction: Before installing *Homebrew*, *Xcode* must be installed.
Run **`$ which g++`** to see if ***Xcode*** installed or not. If not, run **`$ xcode-select --install`** to install ***Xcode***.

Once ***Xcode*** is installed successfully, ***Homebrew*** can be installed using the command below -  
**`$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"`**

To verify if Homebrew has been successfully installed or not check the current version by the command below -  
**`$ brew -v`**

<br>

## :mag: ***Brew*** commands for installing Libraries and Applications
  * [install ***Java*** from ***AdoptOpenJDK*** provider via ***brew***](#adoptopenjdk)
  * [install ***Intellij Idea Community Edition*** via ***brew***](#intellij-idea-ce)
  * [install ***Google Chrome*** via ***brew***](#google-chrome)
  * [install ***Firefox*** via ***brew***](#firefox)  
  
---

## <a name="adoptopenjdk">Insatlling AdoptOpenJDK using brew</a>
Some can find installing **Java** very confusing like setting up the path and etc. Well, ***brew*** is here to rescue.
So, to install the ***Java*** on your **OS X** just follow one of the options below.

### Option 1. Install latest Java version from AdoptOpenJDK provider
By running 2 commands below ***brew*** will download the ***latest version of Java*** from ***AdoptOpenJDK*** provider and will set the ***$JAVA_HOME*** path for you.  
   * **`$ brew tap AdoptOpenJDK`**  
   * **`$ brew cask install adoptopenjdk`**  
  

### Option 2. Install a specific Java version from AdoptOpenJDK provider
By running 2 commands below ***brew*** will download the ***provided version of Java*** from ***AdoptOpenJDK*** provider and will set the ***$JAVA_HOME*** path for you.  
   * **`$ brew tap AdoptoOpenJDK`**  
   * **`$ brew cask install adoptopenjdk8/9/10/11`**  
   
*note:* **`$ brew tap ...`** is optional if you have run this command before to ***tap*** a repository.  

---


## <a name="intellij-idea-ce">Insatlling Intellij Idea Community Edition using brew</a>
To install the **Intellij Idead Community Edition** on your **OS X** just run the command below. ***Brew*** will download the latest version of **Intellij Idead Community Edition** and will place it in under ***Applications***.  
**`$ brew cask install intellij-idea-ce`**  

---

## <a name="google-chrome">Insatlling Google Chrome using brew</a>
To install the **Google Chrome** on your **OS X** just run the command below. ***Brew*** will download the latest version of   **Google Chrome** and will place it in under ***Applications***.  
**`$ brew cask install google-chrome`**

---

## <a name="firefox">Insatlling Firefox using brew</a>
To install the **Firefox** on your **OS X** just run the command below. ***Brew*** will download the latest version of **Firefox** and will place it in under ***Applications***.  
**`$ brew cask install firefox`**  

---
