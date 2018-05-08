FROM nginx:1

RUN rm /etc/nginx/conf.d/default.conf

ADD nginx.conf /etc/nginx/nginx.conf
ADD conf.d/* /etc/nginx/conf.d/
ADD sites.d/* /etc/nginx/sites.d/
ADD ssl/default/* /etc/nginx/ssl/default/

WORKDIR /var/www

EXPOSE 80 443
