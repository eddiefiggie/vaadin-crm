# Simple-CRM

***Credit:***

These are my notes having followed a tutorial from Vaadin.  Their comprehensive tutorial can be found here:  https://vaadin.com/learn/tutorials/modern-web-apps-with-spring-boot-and-vaadin/importing-running-and-debugging-a-java-maven-project-in-intellij-idea

***Setup Guide:***

_**Install Java 11 JDK (Most Recent LTS)**_

The easiest way to install the Java SDK is to use SDKMAN.  Here is a link to help set this up: https://sdkman.io/install

Now with SDKMAN ready to go, now we can install the Java JDK of our liking.  I suggest Amazon Corretto 11 which is based on OpenJDK.  You can evaluate the various versions available for install by typing the following:

sdk list java

Find the most recent version 11 build (current LTS) and install it as follows:

sdk install java 11.0.8-amzn

This installs the JDK on an Ubuntu system in:

~/.sdkman/candidates/java/current

The "current" folder will update based on the JDK version you have as "default".  This will set up all of the appropriate system variables for you.  With SDKMAN you can easily hop around from build to build.

_**Install Maven**_

On Ubuntu, at the command line type:

sudo apt policy maven

This will show you which build is packaged within the repositoy.  Assuming it's current (validate here: https://maven.apache.org/download.cgi), simply install with:

sudo apt install maven

Confirm the installation with the following:

mvn -version

The result will be something like:

Apache Maven 3.6.3
Maven home: /usr/share/maven
Java version: 11.0.8, vendor: Amazon.com Inc., runtime: /home/eddiefiggie/.sdkman/candidates/java/11.0.8-amzn
Default locale: en_US, platform encoding: UTF-8
OS name: "linux", version: "5.4.0-7634-generic", arch: "amd64", family: "unix"

_**Install Node.js**_

To install Node.js and the Node Package Manager use the following:

sudo apt install nodejs

Confirm the installation with:

nodejs -v

Now install NPM:

sudo apt install npm

_**Install Git**_

Installing Git on Ubuntu is simple, use the following:

sudo apt install git

Then confirm your installation with:

git --version


_**Install Intellij IDEA**_

Installing IntelliJ IDEA on Ubuntu as a snap can be done as follows:

https://blog.jetbrains.com/idea/2017/11/install-intellij-idea-with-snaps/

***Importing a Maven project into IntelliJ***

Build a Spring Boot starter project:
https://vaadin.com/start/v14


