FROM ubuntu:focal
ENV DEBIAN_FRONTEND=noninteractive
RUN apt-get update \
    && apt-get install -y apache2 git
RUN git clone https://github.com/SEOMW/docker_example.git
RUN cp -r docker_example/* /var/www/html/
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
