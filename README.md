# Metrics for Developers #

## About ##

Metrics workshop at [Booster](http://www.boosterconf.no/) 2015.

## Requirements ##

* Git 1.7.10+
* [Apache Maven](http://maven.apache.org/) 3.1.x
* Java 8

## Getting Started ##

* Download source as [ZIP](https://github.com/kantega/metrics-workshop/archive/master.zip) or clone it:

        git clone https://github.com/kantega/metrics-workshop.git

* Download [Java JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/index.html).
* Set System Variable JAVA_HOME to install location of JDK.
* (Optional) Install Maven by running Maven Wrapper:

        (Windows)    mvnw.bat
        (Linux/Mac)  ./mvnw

## Starting workshop ##

__(alt 1) Maven__

    mvn clean install
    cd webapp
    mvn jetty:run

Open up your favorite browser to [http://localhost:8080/workshop-ui/](http://localhost:8080/workshop-ui/).

__(alt 2) Maven Wrapper__

    mvnw(.bat) clean install
    cd webapp
    mvnw(.bat) jetty:run

Open up your favorite browser to [http://localhost:8080/workshop-ui/](http://localhost:8080/workshop-ui/).

__(alt 3) IntelliJ IDEA & Maven__

1. Download and install [Maven](https://maven.apache.org/download.html)
2. Download and install [IDEA](https://www.jetbrains.com/idea/download)
3. Start IDEA, Open Project -> select metrics-workshop/pom.xml
4. Click Build -> Make Project
5. Click 'Maven Project' on Right menu bar -> webapp -> Plugins -> Right click jetty:run -> Debug 'webapp' \[jetty:run\]
    * If asked about "No Maven installation..", click 'configuration dialog', and set 'Maven home location' to installed Maven home dir
6. Open up your favorite browser to [http://localhost:8080/workshop-ui/](http://localhost:8080/workshop-ui/)


__(alt 4) Eclipse (Luna required)__

1. Download and install [Eclipse IDE for Java EE Developers (Luna)](https://eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/lunar)
2. Import -> Maven -> Existing Maven Projects
    * Root Directory: Select metrics-workshop path -> Next -> Finish
3. Under 'Project Explorer Window' Select project webapp, then go to Run Menu -> Debug As -> Maven Build (first one)
    * Write 'install jetty:run' in Goals -> Debug
    * To modify settings afterwards go to Run Menu -> Debug Configuration
4. Open up your favorite browser to [http://localhost:8080/workshop-ui/](http://localhost:8080/workshop-ui/)
