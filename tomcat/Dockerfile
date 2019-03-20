FROM huahua5404/minial-java:1.8 

MAINTAINER tchua

ADD  apache-tomcat-8.5.38.tar.gz /usr/local/
RUN  rm -rf /usr/local/apache-tomcat-8.5.38/webapps/ROOT/* \
     && echo "<h3>This is tomcat:v2</h3>" > /usr/local/apache-tomcat-8.5.38/webapps/ROOT/index.html
EXPOSE 8080
ENTRYPOINT ["/usr/local/apache-tomcat-8.5.38/bin/catalina.sh","run"]


