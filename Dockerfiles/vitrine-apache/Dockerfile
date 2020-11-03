FROM debian

RUN apt update -y -q
RUN apt upgrade -y -q
RUN apt install apache2 -y

COPY www/index.html /var/www/html

EXPOSE 80

CMD apache2ctl -D FOREGROUND