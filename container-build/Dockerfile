# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

#EXPOSE 80

EXPOSE 8080

# This stuff is needed to ensure a clean start
#RUN rm -rf /run/httpd && mkdir /run/httpd

RUN chgrp -R 0 /run/httpd /usr/sbin/httpd &&\
 chmod -R g=u /run/httpd /usr/sbin/httpd


#USER root
USER 1001


