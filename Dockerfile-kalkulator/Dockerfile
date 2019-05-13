FROM ubuntu:16.04

ENV UBUNTU_FRONTEND=noninteractive

RUN apt-get update && \
 apt-get install -y tzdata && \
 apt-get install -y apache2 && \
 apt-get install -y apache2-utils && \
 #apt-get install -y mysql-server && \
 apt-get install -y php && \
 apt-get install -y libapache2-mod-php && \
 apt-get install -y git

RUN rm -rf /var/www/html/*

RUN git clone http://github.com/rivawahyuda/kalkulator /var/www/html

RUN apt-get clean
WORKDIR /var/www/html
CMD ["apache2ctl","-D","FOREGROUND"]
EXPOSE 80


# sudo docker build -t calculator .
# sudo docker image ls
# sudo docker run -d -p 4000:80 calculator
