FROM  ubuntu:latest
 MAINTAINER bikash9089@gmail.com
Run apt update -y
 RUN apt install -y apache2 \
  zip\
  unzip
  ADD https://www.free-css.com/assets/files/free-css-templates/download/page265/shine.zip /var/www/html/
 WORKDIR /var/www/html/
 RUN unzip shine.zip
 RUN cp -rvf shine/* .
 RUN rm -rf shine shine.zip
 CMD ["/usr/sbin/apache2", "-D", "FOREGROUND"]
 EXPOSE 80
