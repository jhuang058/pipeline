FROM tomcat:8-jre8-alpine

#cleans the webapps folder
RUN rm -rf /usr/local/tomcat/webapps/*

#Copy takes the artifact from the file directory where the docker file is and places it in the Tomcat webapps folder
COPY HelloServlets.war /usr/local/tomcat/webapps/HelloServlets.war

#will "run catalina.sh" on the command line when the container is spun up. This will start tomcat with whatever...
CMD ["catalina.sh", "run"]