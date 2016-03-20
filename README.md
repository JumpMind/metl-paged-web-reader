The Paged Web Reader is a custom component designed to work with METL 1.1.1. 

This component extends the built in Web component by adding support for a specific type of web service pagination. 

Use this component to break up requests for data into multiple smaller requests(pages). This is helpful when querying large data sets. Each smaller paged response is sent as a message to downstream components increasing the speed of your flow while reducing memory requirements.

For more information on using the Paged Web Reader component, see the [Wiki](https://github.com/JumpMind/metl-paged-web-reader/wiki).

## Build Me, Run Me

This project requires the Java JDK to build and run.  The build currently generates a jar file 
which can be dropped into a metl plugin directory.

### Build
~~~~~
./gradlew jar
~~~~~

### Install
~~~~~
cp ./build/libs/metl-paged-web-reader.jar /opt/metl/plugins/.
service metl restart
~~~~~

### Develop
To develop in [Eclipse](http://eclipse.org) run the following and import the projects:
~~~~~
./gradlew develop
~~~~~
