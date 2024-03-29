FROM tomcat:9-jre8

WORKDIR /usr/local/tomcat

COPY target/docker-java-sample-webapp-1.0-SNAPSHOT.war webapps/ROOT.war

# Expose the default Tomcat port
EXPOSE 8080


CMD ["catalina.sh", "run"]



