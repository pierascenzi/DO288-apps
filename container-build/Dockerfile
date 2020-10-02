# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

#EXPOSE 80
EXPOSE 8080

RUN sed -i 's/Listen 80/Listen 8080/g' /etc/httpd/conf/httpd.conf &&\
 chgrp -R 0 /run/httpd /etc/httpd/logs/ &&\
 chmod -R g=u /run/httpd /etc/httpd/logs/

#USER root
USER 1001

