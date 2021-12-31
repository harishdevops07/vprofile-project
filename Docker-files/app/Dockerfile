FROM tomcat:8-jre11
LABEL "Project"="Vprofile"
LABEL "Author"="Harish"
ENV AUTHOR_NAME="Harish Rawat"
RUN rm -rf /usr/local/tomcat/webapps/*
COPY target/*.war /usr/local/tomcat/webapps/ROOT.war
EXPOSE 8080
CMD ["catalina.sh", "run"]
WORKDIR /usr/local/tomcat/
VOLUME /usr/local/tomcat/webapps
MAINTAINER $AUTHOR_NAME