# startUsingJavaJUnit

A simple Java JUnit 4 project to check Java and Maven are installed correctly.

[For a Java JUnit 5 project look here](https://github.com/eviltester/startUsingJavaJUnit5)

This project demonstrates:

- Maven Setup
- JUnit execution

Clone or download the project.

Pre-requisites:

* JDK Installed
* MAVEN Installed

## Pre-requisite Install Instructions

Install instructions can be found in `speedrun_install_java_checklist.md`

Read the [Speedrun Install Java Checklist](https://github.com/eviltester/startUsingJavaJUnit/blob/master/speedrun_install_java_checklist.md)
for more details.

## Usage

In the root folder where the `pom.xml` resides, type:

~~~~~~~~
mvn test
~~~~~~~~

And you should see something like:

~~~~~~~~
[INFO] Scanning for projects...
[INFO]
[INFO] ------------------------------------------------------------------------
[INFO] Building MyFirstJUnitTest 1.0
[INFO] ------------------------------------------------------------------------
[INFO]

... blah blah blah ...

-------------------------------------------------------
 T E S T S
-------------------------------------------------------
Running com.javafortesters.junit.MyFirstTest
Tests run: 1, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.043 sec

Results :

Tests run: 1, Failures: 0, Errors: 0, Skipped: 0

[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time: 1.764 s
[INFO] Finished at: 2016-09-30T10:55:03+01:00
[INFO] Final Memory: 9M/245M
[INFO] ------------------------------------------------------------------------
~~~~~~~~

If you see the `BUILD SUCCESS` then everything has installed properly.

## About

Author: [Alan Richardson](https://www.linkedin.com/in/eviltester/)

* [EvilTester.com](https://eviltester.com)
* [Compendium Developments](https://compendiumdev.co.uk)

- [A Java JUnit 5 version of this project is available](https://github.com/eviltester/startUsingJavaJUnit5)
    - [github.com/eviltester/startUsingJavaJUnit5](https://github.com/eviltester/startUsingJavaJUnit5)