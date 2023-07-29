# Generic Java Install Speedrun checklist

*Basic steps:*

- Install Java and supporting tools
    - install Java JDK
    - install Maven
    - check Java and Maven work by running a sample test
- Install IntelliJ
    - check IntelliJ works by running the sample test
        
This checklist contains instructions for Windows and Mac.

---

## Install Videos

*Windows Install Videos*

* [YouTube Video Showing the Java Install on Windows 10](https://youtu.be/1bDd5B8TA2g)
* https://youtu.be/1bDd5B8TA2g (Updated November 2017)
    * previous version https://www.youtube.com/watch?v=j-46lYWAHF0  (4 Oct 2016)

*Mac Install Videos*

* [YouTube Video Showing the Java Install on a Mac](https://youtu.be/vHGdjKuXKAs)
* https://youtu.be/vHGdjKuXKAs  (Updated November 2017)
    * previous version https://youtu.be/ff5ZsthcSZw (4 Oct 2016)

---

## Install Java Pre-requisites

* `[ ]` Check what you need to install by typing console commands
    * `[ ]` "javac -version"
          - if it fails then you need to install a Java JDK
    * `[ ]` "mvn -version"
          - if it fails then you need to install maven
          
---

# Windows Install Speedrun checklist

---

## Install Java JDK, Maven and IntelliJ Using Chocolatey

The simple way is to install the apps is to use Chocolatey

- Follow Install instructions [chocolatey.org/install](https://chocolatey.org/install)
- Using the packages [chocolatey.org/packages](https://chocolatey.org/packages)
- find what we want: (I find the chocolatey search isn't always the best so I use Google as well "site:chocolatey.org Java SE 9 JDK") (or chocolate search "tag:jdk")
    - `choco install openjdk`
    - `choco install maven`
    - `choco install intellijidea-community`


---

### Longer Instructions for Install on Windows

If you used Chocolatey then you can skip this and move to the 'Check the install on Windows' section.

* `[ ]` Download Java SDK from either Adoptium.net or Oracle 
    * `[ ]` Recommended Adoptium install https://adoptium.net/
    * `[ ]` Oracle's Open JDK https://openjdk.org/

---

* `[ ]` Install The Java JDK
    * `[ ]` Windows
        * `[ ]` check Java JDK installed by typing `javac -version` in a new command line
        * `[ ]` add the JDK "\bin" folder to the path if it hasn't been added
        * `[ ]` create a JAVA_HOME environment variable for the root path of the JDK

---

* `[ ]` Install Maven
    * `[ ]` Download Maven https://maven.apache.org/download.cgi
    * `[ ]` Windows
        * Follow the install instructions https://maven.apache.org/install.html
        * `[ ]` Unzip maven to a directory (avoid one with spaces in it)
            - e.g. `C:\maven_3_9_3`
        * `[ ]` add `C:\maven_3_9_3\bin` to the `PATH` in System Variables
        * `[ ]` check installed by typing `mvn -version` into a new command window

---

* `[ ]` with everything now installed, check the environment variables by displaying them on the console
    * `[ ]` Windows
        * `[ ]` `echo %JAVA_HOME%`
        * `[ ]` `echo %PATH%`

---

* Install IntelliJ
    * `[ ]`  download IntelliJ Community Edition from https://www.jetbrains.com/idea
    * `[ ]`  install it

---


## Check the install on Windows

* The following commands should now run from a command line - you might need to start a new command line or possibly reboot to refresh your window settings after installing JDK and Maven.
    * `[ ]` "javac -version"
    * `[ ]` "mvn -version"
    
If either of the above fail then you have not installed Java or Maven.

* `[ ]` Download JUnit Test Project (this has a simple pom.xml and a basic test to run)
    * `[ ]` visit https://github.com/eviltester/startUsingJavaJUnit
    * `[ ]` download the zip file and unzip somewhere

* `[ ]` run my first test from the command line
    * `[ ]` use the command line to "cd" to the directory you unarchived the source code to
    * `[ ]` `mvn test`

If it runs successfully then you have Java and Maven Installed in Windows.

---

## Open and Run the source code from IntelliJ

* `[ ]`  create new project from existing sources
* `[ ]`  open the `pom.xml` from the folder that we  placed the downloads from https://github.com/eviltester/startUsingJavaJUnit
    * `[ ]` in IntelliJ use 'Open Project' and select the folder, or the `pom.xml` file
* `[ ]`  we may need to configure IntelliJ to use the Java SDK we installed earlier, if so, follow the IntelliJ prompts
    * `[ ]` you may need to tell intellij where the SDK is,
        - use the project settings to create an new SDK config
          using the `JAVA_HOME` path above
* `[ ]`  right click on the test and 'run' the test
* `[ ]`  if it passes it means that Java, Maven, IntelliJ are all now installed and ready to use

---
    
# Mac Install Speedrun checklist - Homebrew

## Use HomeBrew to install Java JDK and Maven

* `[ ]` install homebrew from http://brew.sh/
* `[ ]` `brew update`
* `[ ]` install jdk with one of :
    - Adoptium.net version `brew install --cask temurin`
    - Oracle Open JDK version `brew install openjdk`
* `[ ]` install maven with `brew install maven`

You can also use SDKMan to manage and install different versions of java SDK: https://sdkman.io/

---

* `[ ]` everything is installed, check the environment variables by displaying them on the console
    * `[ ]` Mac
        * `[ ]` `echo $JAVA_HOME`
        * `[ ]` `echo $PATH`

---

* `[ ]` Download JUnit Test Project (this has a simple pom.xml and a basic test to run)
    * `[ ]` visit https://github.com/eviltester/startUsingJavaJUnit
    * `[ ]` download the zip file and unzip somewhere

* `[ ]` run my first test from the command line
    * `[ ]` use the command line to "cd" to the directory you unarchived the source code to
    * `[ ]` `mvn test`

If it runs successfully then you have Java and Maven Installed on Mac.

---


## Install IntelliJ Community Edition on Mac 

You can install IntelliJ using Homebrew as well by typing:

* `[ ]` `brew install --cask intellij-idea-ce`

Or you can install it like a normal Mac application using the instructions below.

* `[ ]` install IntelliJ IDE Community Edition,
    * visit the web site https://www.jetbrains.com/idea/ 
    * download and install the Community Edition
    
* `[ ]` open the 'startUsingJavaJUnit' project in IntelliJ and run the test from the IDE to ensure IntelliJ and JDK and Maven are all working together.    

---

Generic Links:
==============

+ Download Java SDK From
    - Adoptium (recommended): https://adoptium.net/
    - Oracle:  https://openjdk.org/

+ Download Maven From
    * http://maven.apache.org/download.cgi

---

+ sample JUnit test project from
   * JUnit 4 - https://github.com/eviltester/startUsingJavaJUnit
   * JUnit 5 - https://github.com/eviltester/startUsingJavaJUnit5

+ Download IntelliJ from
    * http://www.jetbrains.com/idea/download/

+ Mac HomeBrew and Cask
    * http://brew.sh
    * https://caskroom.github.io

---

+ How to install Java on Mac
    * http://stackoverflow.com/questions/24342886/how-to-install-java-8-on-mac
    
+ How do uninstall Java on Mac
    * https://www.java.com/en/download/help/mac_uninstall_java.xml
    * http://docs.oracle.com/javase/8/docs/technotes/guides/install/mac_jdk.html

