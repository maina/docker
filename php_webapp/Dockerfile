FROM ubuntu:14.04
MAINTAINER James Bugara "bugara.james@yahoo.com"
RUN apt-get update && apt-get install -y apache2
ENV APACHE_RUN_USER www-data
ENV APACHE_RUN_GROUP www-data
ENV APACHE_LOG_DIR /var/log/apache2
ONBUILD ADD . /var/wwww/
ENTRYPOINT ["usr/sbin/apache2ctl"]
CMD ["-D","FOREGROUND"]
EXPOSE 80
