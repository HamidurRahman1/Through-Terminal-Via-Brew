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

## :mag: ***Brew*** commands to install Libraries and Applications
  * [***Jenkins***](#jenkins) 
  * [***Maven***](#maven) 
  * [***Node***](#node) 
  * [***MySQL***](#mysql) 
  * [***MongoDB Community Edition***](#mongodb-ce) 
  * [***Google Chrome Driver***](#google-chrome-driver) 
  * [***Java*** from ***AdoptOpenJDK*** provider](#adoptopenjdk)
  * [***Python***](#adoptopenjdk)
  * [***Anaconda***](#anaconda)
  * [***Intellij Idea Ultimate Edition***](#intellij-idea)
  * [***Intellij Idea Community Edition***](#intellij-idea-ce)
  * [***PyCharm Ultimate Edition***](#pycharm)
  * [***PyCharm Community Edition***](#pycharm-ce)
  * [***Atom***](#atom)
  * [***Google Chrome***](#google-chrome)
  * [***Firefox***](#firefox)  

---

## <a name="jenkins">Install Jenkins</a>
To install Jenkins on your OS X just run the commands below. Brew will download the latest version of Jenkins.  
**`$ brew install jenkins-lts`**  

By default Jenkins create an administrator and generate a password. The password can be found by running  
**`$ cat /Users/{username}/.jenkins/secrets/initialAdminPassword`**  

### Start Jenkins service by running  
**`$ brew services start jenkins-lts`**  
Jenkins will be using port 8080 so we can check if it's running by going to http://localhost:8080/

### Stop Jenkins service by running  
**`$ brew services stop jenkins-lts`**  

---

## <a name="maven">Install Maven</a>
To install Maven on your OS X just run the commands below. Brew will download the latest version of Maven.  
**`$ brew install maven`**  

### Verify maven is installed by running  
**`$ mvn -v`**

---

## <a name="node">Install NodeJS and NPM</a>
To install NodeJS and NPM on your OS X just run the command below. Brew will download the latest version of NodeJS and NPM.   
**`$ brew install node`**  

### Verify NodeJS is installed by running  
**`$ node -v`**  

### Verify NPM is installed by running  
**`$ npm -v`**

---

## <a name="mysql">Install MySQL </a>
To install MySQL on your OS X just run the command below. Brew will download the latest version of MySQL.   
**`$ brew install mysql`**  

### Secure and set root account's password by running   
**`$ mysql_secure_installation`**  

### Start MySQL service by running  
**`$ brew services start mysql`**  

### Stop MySQL service by running  
**`$ brew services stop mysql`**  

### Verify MySQL is installed by running  
**`$ mysql --version`**  

### Login to MySQL via terminal by running
**`$ mysql -u root -p`**  

---

## <a name="mongodb-ce">Install MongoDB Community Edition</a>
To install MongoDB Community Edition on your OS X just run the commands below. Brew will download the latest version of MongoDB Community Edition.  
**`$ brew tap mongodb/brew`**  
**`$ brew install mongodb-community`**  

### Start MongoDB service by running  
**`$ brew services start mongodb-community`**  

### Stop MongoDB service by running  
**`$ brew services stop mongodb-community`**  

### Verify MongoDB is installed by running  
**`$ mongod --version`**

---

## <a name="adoptopenjdk">Insatll AdoptOpenJDK using brew</a>
Some can find installing Java very confusing like setting up the path and etc. Well, brew is here to rescue. So, to install the Java on your OS X just follow one of the options below.

### Option 1. Install latest Java version from AdoptOpenJDK provider
By running 2 commands below brew will download the latest version of Java from AdoptOpenJDK provider and will set the ***$JAVA_HOME*** path for you.  
   * **`$ brew tap AdoptOpenJDK`**  
   * **`$ brew cask install adoptopenjdk`**  
  

### Option 2. Install a specific Java version from AdoptOpenJDK provider
By running 2 commands below brew will download the provided version of Java from AdoptOpenJDK provider and will set the ***$JAVA_HOME*** path for you.  
   * **`$ brew tap AdoptoOpenJDK`**  
   * **`$ brew cask install adoptopenjdk8/9/10/11`**  
   
### Verify Java is installed by running  
**`$ java --version`**   
   
*note:* **`$ brew tap X`** is optional to install something from that repository ***X***. If you have run this command before to ***tap*** repository ***X***.  

---

## <a name="python">Insatll Python using brew</a>
To install the Python on your OS X just follow one of the options below.

### Option 1. Install latest Python version
By running the command below brew will download the latest version of Python for you.  
   * **`$ brew install python`**  
  

### Option 2. Install a specific Python version
By running the command below brew will download the provided version of Python for you.  
   * **`$ brew install python2/3`**  
   
### Verify Python is installed by running  
**`$ python3 --version`**  
or  
**`$ pythonX --version`**  
Where **X** is 2/3 or future released version number

---

## <a name="anaconda">Insatll Anaconda using brew</a>
To install Anaconda on your OS X just run the command below. Brew will download the latest version of Intellij Idea Ultimate Edition and will place it in under Applications.  
**`$ brew cask install anaconda`**  

### Verify Anaconda is installed by running  
**`$ conda --version`** 

---

## <a name="google-chrome-driver">Install Google Chrome Driver</a>
To install Google Chrome Driver on your OS X just run the command below. Brew will download the latest version of Chrome Driver.  
**`$ brew cask install chromedriver`**  

### Verify ChromeDriver is installed by running  
**`$ chromedriver --version`**

---

## <a name="intellij-idea">Insatll Intellij Idea Ultimate Edition using brew</a>
To install Intellij Idea Ultimate Edition on your OS X just run the command below. Brew will download the latest version of Intellij Idea Ultimate Edition and will place it in under Applications.  
**`$ brew cask install intellij-idea`**  

---

## <a name="intellij-idea-ce">Insatll Intellij Idea Community Edition using brew</a>
To install Intellij Idea Community Edition on your OS X just run the command below. Brew will download the latest version of Intellij Idea Community Edition and will place it in under Applications.  
**`$ brew cask install intellij-idea-ce`**  

---

## <a name="pycharm">Insatll PyCharm Ultimate Edition using brew</a>
To install PyCharm Ultimate Edition on your OS X just run the command below. Brew will download the latest version of PyCharm Ultimate Edition and will place it in under Applications.  
**`$ brew cask install pycharm`**  

---

## <a name="pycharm-ce">Insatll PyCharm Community Edition using brew</a>
To install PyCharm Community Edition on your OS X just run the command below. Brew will download the latest version of Intellij Idea Community Edition and will place it in under Applications.  
**`$ brew cask install pycharm-ce`**  

---

## <a name="atom">Insatll Atom Editor using brew</a>
To install Atom on your OS X just run the command below. Brew will download the latest version of Atom and will place it in under Applications.  
**`$ brew cask install atom`**

---

## <a name="google-chrome">Insatll Google Chrome using brew</a>
To install Google Chrome on your OS X just run the command below. Brew will download the latest version of Google Chrome and will place it in under Applications.  
**`$ brew cask install google-chrome`**

---

## <a name="firefox">Insatll Firefox using brew</a>
To install Firefox on your OS X just run the command below. Brew will download the latest version of Firefox and will place it in under Applications.  
**`$ brew cask install firefox`**  

---
