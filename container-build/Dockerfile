# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

#EXPOSE 80

EXPOSE 8080

# This stuff is needed to ensure a clean start
#RUN rm -rf /run/httpd && mkdir /run/httpd

RUN sed -i "s/Listen 80/Listen 8080/g" /etc/httpd/conf/httpd.conf &&\ 
 chgrp -R 0 /run/httpd /var/log/httpd &&\
 chmod -R g=u /run/httpd /var/log/httpd

#USER root
USER 1001
