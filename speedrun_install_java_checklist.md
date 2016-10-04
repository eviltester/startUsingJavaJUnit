# Generic Java Install Speedrun checklist

*Basic steps:*

- Install Java and supporting tools
    - install Java JDK
    - install Maven
    - check Java and Maven work by running a sample test
- Install IntelliJ
    - check IntelliJ works by running the sample test
        
This checklist contains instructions for Windows and Mac.
    
    
# Windows Install Speedrun checklist

## Install Java Pre-requisites - Install Java Speedrun on Windows

* `[ ]` Check what you need to install by typing console commands
    * `[ ]` "javac -version"
          - if it fails install java jdk
    * `[ ]` "mvn -version"
          - if it fails install maven

* `[ ]` Download Java
    * `[ ]` search for "download java sdk" (do not install the normal JRE from java.com)
         - http://www.oracle.com/technetwork/java/javase/downloads/index.html

* `[ ]` Install Java JDK
    * `[ ]` Windows
        - e.g. `C:\Program Files\Java\jdk1.8.0_102`
        * `[ ]` add the Java "\bin" folder to the path if it hasn't been added
           e.g. `C:\Program Files\Java\jdk1.8.0_102\bin`
        * `[ ]` create a JAVA_HOME environment variable while there for the root path
            e.g. `C:\Program Files\Java\jdk1.8.0_102`
            - some people add a `JDK_HOME` for the root path as well (I haven't done this)
        * `[ ]` check Java JDK installed by typing `javac -version` in a new command line

* `[ ]` Install Maven
    * `[ ]` Download Maven http://maven.apache.org/download.html#Installation
    * `[ ]` Windows
        * `[ ]` Unzip maven to a directory (avoid one with spaces in it)
            - e.g. `C:\maven_3_3_9`
        * `[ ]` add `C:\maven_3_3_9\bin` to the `PATH` in System Variables
        * `[ ]` check installed by typing `mvn -version` into a new command window

* `[ ]` everything is installed, check the environment variables by displaying them on the console
    * `[ ]` Windows
        * `[ ]` `echo %JAVA_HOME%`
        * `[ ]` `echo %PATH%`


* `[ ]` Download JUnit Test Project (this has a simple pom.xml and a basic test to run)
    * `[ ]` visit https://github.com/eviltester/startUsingJavaJUnit
    * `[ ]` download the zip file and unzip somewhere

* `[ ]` run my first test from the command line
    * `[ ]` use the command line to "cd" to the directory you unarchived the source code to
    * `[ ]` `mvn test`

If it runs successfully then you have Java and Maven Installed in Windows.

## Install IntelliJ for Java  - Install IntelliJ Java Speedrun on Windows


* `[ ]`  download IntelliJ Community Edition from https://www.jetbrains.com/idea
* `[ ]`  install it
* `[ ]`  new project from existing sources
* `[ ]`  open the `pom.xml` from the folder that we placed the downloads from https://github.com/eviltester/startUsingJavaJUnit
* `[ ]`  we may need to configure IntelliJ to use the Java SDK we installed earlier, if so, follow the IntelliJ prompts
    * `[ ]` you may need to tell intellij where the SDK is,
        - use the project settings to create an new SDK config
          using the `JAVA_HOME` path above
* `[ ]`  right click on the test and 'run' the test
* `[ ]`  if it passes it means that Java, Maven, IntelliJ are all now installed and ready to use
    
    
# Mac Install Speedrun checklist - Homebrew

## Use HomeBrew to install Java JDK and Maven

* `[ ]` install homebrew from http://brew.sh/
* `[ ]` `brew update`
* `[ ]` install jdk with `brew cask install java`
* `[ ]` install maven with `brew install maven`

* `[ ]` everything is installed, check the environment variables by displaying them on the console
    * `[ ]` Windows
        * `[ ]` `echo $JAVA_HOME`
        * `[ ]` `echo $PATH`

* `[ ]` Download JUnit Test Project (this has a simple pom.xml and a basic test to run)
    * `[ ]` visit https://github.com/eviltester/startUsingJavaJUnit
    * `[ ]` download the zip file and unzip somewhere

* `[ ]` run my first test from the command line
    * `[ ]` use the command line to "cd" to the directory you unarchived the source code to
    * `[ ]` `mvn test`

If it runs successfully then you have Java and Maven Installed on Mac.

## Install IntelliJ Community Edition on Mac 

* `[ ]` install IntelliJ IDE Community Edition,
    * visit the web site https://www.jetbrains.com/idea/ 
    * download and install the Community Edition
    
* `[ ]` load the 'startUsingJavaJUnit' project into IntelliJ and run the test from the IDE to ensure IntelliJ and JDK and Maven are all working together.    


Generic Links:
==============

+ Download Java SDK From
http://www.oracle.com/technetwork/java/javase/downloads/index.html
  - 1.8 http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
  - 1.7 http://www.oracle.com/technetwork/java/javase/downloads/jdk7-downloads-1880260.html

+ Download Maven From
    * http://maven.apache.org/download.cgi

+ sample JUnit test project from
    * https://github.com/eviltester/startUsingJavaJUnit

+ Download IntelliJ from
    * http://www.jetbrains.com/idea/download/

+ Mac HomeBrew and Cask
    * http://brew.sh
    * https://caskroom.github.io/

+ How to install Java on Mac
    * http://stackoverflow.com/questions/24342886/how-to-install-java-8-on-mac
    
+ How do uninstall Java on Mac
    * https://www.java.com/en/download/help/mac_uninstall_java.xml
    * http://docs.oracle.com/javase/8/docs/technotes/guides/install/mac_jdk.html