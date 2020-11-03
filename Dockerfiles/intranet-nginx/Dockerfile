FROM debian

RUN apt update -y -q
RUN apt upgrade -y -q
RUN apt install nginx -y

RUN rm /var/www/html/index.nginx-debian.html
RUN echo "daemon off;" >> /etc/nginx/nginx.conf
COPY www/index.html /var/www/html/index.nginx-debian.html

EXPOSE 80

CMD nginx