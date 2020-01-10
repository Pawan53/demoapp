#Docker file for  apache for demo
FROM centos:7
#MAINTAINER URL---mETADATA
RUN yum -y update
#RUN yum -y install httpd php php-gd php-mysql
ADD scripts /opt
RUN chmod 755 /opt/*
RUN /opt/packages
ADD code /var/www/html
#COPY code/* /var/www/html
ENV MY_DB_HOST_WRITE=test
#EXPOSE---METADATA
EXPOSE 80
CMD ["httpd","-D","FOREGROUND"]  