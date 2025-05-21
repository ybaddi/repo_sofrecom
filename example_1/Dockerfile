FROM  ubuntu:24.04

# information of the editor
LABEL version="1.0.0"
LABEL maintainer="baddi"

RUN apt update 
RUN apt-get install -y apache2
RUN apt install -y mysql-server

ENV APACHE_RUN_USER www-data
ENV TZ=UTC

EXPOSE 80
# ------------------------------------

CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
