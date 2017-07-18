FROM mysql
ENV MYSQL_ROOT_PASSWORD root
COPY createdb.sql /opt/
COPY init.sh /opt/
RUN chmod +x /opt/init.sh
WORKDIR /opt
ENTRYPOINT /opt/init.sh && bin/sh



#FROM openjdk:alpine
#COPY C://images/Sample.java /sources/
#WORKDIR /sources
#RUN javac Sample.java
#RUN rm Sample.java
#CMD java 	Sample


#FROM ubuntu
#ARG MESSAGE_ARG='Building message'
#ENV message $MESSAGE_ARG
#LABEL Author=dboyko Company="Slice"
#RUN echo 'Building image …'
#COPY docs/ /docs/
#WORKDIR /docs
#RUN cat instructions.txt
#ENTRYPOINT ["/bin/sh"]
#RUN echo $message