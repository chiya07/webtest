FROM centos:7
MAINTAINER chiya07@gmail.com
RUN yum -y install httpd
ADD code /var/www/html
ENV DB_NAME=test DB_PORT=3306
EXPOSE 80
CMD ["apachectl","-D","FOREGROUND"]