FROM ubuntu:latest
RUN apt-get -y update
RUN apt-get -y install tzdata
ENV TZ=Asia/Kolkata
ADD config /opt
RUN apt-get -y install `cat /opt/packages`
ADD code /var/www/html
EXPOSE 80
ENTRYPOINT ["nginx", "-g", "daemon off;"]