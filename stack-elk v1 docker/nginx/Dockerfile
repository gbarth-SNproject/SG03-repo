FROM nginx:stable

ADD conf/nginx.conf /etc/nginx/

RUN usermod -u 1000 www-data
EXPOSE 80
EXPOSE 443

