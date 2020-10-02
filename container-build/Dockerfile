# Use the httpd-parent image as base
FROM quay.io/redhattraining/httpd-parent

#EXPOSE 80
EXPOSE 8080

RUN chgrp -R 0 /run/httpd &&\
 chmod -R g=u /run/httpd

#USER root
USER 1001

