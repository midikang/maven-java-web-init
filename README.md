# web-spring-java-simple
A simple Spring app

# Developer Workspace

[![Contribute](http://beta.codenvy.com/factory/resources/codenvy-contribute.svg)](http://beta.codenvy.com/f?id=hrh4c8gw8tlehd0i)

# Stack to use

FROM [codenvy/ubuntu_jdk8](https://hub.docker.com/r/codenvy/ubuntu_jdk8/)

or


FROM [codenvy/debian_jdk8](https://hub.docker.com/r/codenvy/debian_jdk8/)

# How to run

| #       | Description           | Command  |
| :------------- |:-------------| :-----|
| 1      | Build and copy war | `mvn -f ${current.project.path} clean install && cp ${current.project.path}/target/*.war $TOMCAT_HOME/webapps/ROOT.war` |
| 2      | Run Tomcat      |   `$TOMCAT_HOME/bin/catalina.sh run` |
| 3 | Stop Tomcat      |    `$TOMCAT_HOME/bin/catalina.sh stop` |
| 4 | Tomcat Debug Mode      |    `$TOMCAT_HOME/bin/catalina.sh jpda run` |

# Midi's command

cd /projects/web-java-spring
mvn -f /projects/web-java-spring clean install && cp /projects/web-java-spring/target/*.war $TOMCAT_HOME/webapps/ROOT.war
$TOMCAT_HOME/bin/catalina.sh jpda run

# Go to url
http://node1.beta.codenvy.com:34310/spring/hello# maven java web project template
