FROM tomcat:8.5
COPY ./student* /usr/local/tomcat/webapps
ADD https://s3-us-west-2.amazonaws.com/studentapi-cit/mysql-connector.jar lib/
COPY ./context.xml conf/context.xml
WORKDIR ./bin
EXPOSE 8080
CMD ["./catalina.sh", "run"]
