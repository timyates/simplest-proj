# Vert.x 3.0 Simplest Maven project

This project shows a very simple HelloWorld Vert.x 3.0 project using Maven.

There is a single verticle called `HelloWorldServer` which always returns "Hello World!"".

The pom.xml uses the Maven shade plugin to assemble the application and all it's dependencies into a single "fat" jar.

To build:

    mvn package

To run from command line:

    java -jar target/simplest-project-1.0-SNAPSHOT-fat.jar

You can take that jar and run it anywhere there is a Java 8+ JDK. It contains all the depdendencies it needs so you
don't need to install Vert.x on the target machine.

---

It also contains a Gradle version.

To build:

    ./gradlew shadowJar

To run from command line:

    java -jar build/libs/simplest-proj-1.0-SNAPSHOT-fat.jar