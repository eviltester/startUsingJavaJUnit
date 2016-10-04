# startUsingJavaJUnit

A simple Java JUnit project to check Java and Maven are installed correctly.

Clone or download the project.

Preqrequisites:

* JDK Installed
* MAVEN Installed

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

Read the [Java Install Checklist](https://github.com/eviltester/startUsingJavaJUnit/blob/master/speedrun_install_java_checklist.md)
 for more details.

Author: Alan Richardson

* [JavaForTesters.com](http://javafortesters.com)
* [Compendium Developments](http://compendiumdev.co.uk)
