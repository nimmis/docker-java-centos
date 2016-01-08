## Java with CentOS 7

This is docker images of CentOS 7 with different versions of java

### Loading different versions of java

The different version is determined with the TAG 

The available version are 

* latest                 - currently Oracle Java version 8 JRE
* openjdk-7-jdk          - OpenJDK Java version 7 JDK
* openjdk-7-jre          - OpenJDK Java version 7 JRE
* openjdk-7-jre-headless - OpenJDK Java version 7 JRE headless
* openjdk-8-jdk          - OpenJDK Java version 8 JDK
* openjdk-8-jre          - OpenJDK Java version 8 JRE
* openjdk-8-jre-headless - OpenJDK Java version 8 JRE headless
* oracle-7-jre           - Oracle Java version 7 JRE
* oracle-7-jdk           - Oracle Java version 7 JDK
* oracle-8-jre           - Oracle Java version 8 JRE
* oracle-8-jdk           - Oracle Java version 8 JDK

Example to run a container with OpenJDK version 7 JDK

	`docker run -ti nimmis/java-centos:openjdk-7-jdk`


