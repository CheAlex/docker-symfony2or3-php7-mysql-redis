FROM nginx:1.11

RUN echo "daemon off;" >> /etc/nginx/nginx.conf

RUN echo "upstream php-upstream { server php_fpm:9000; }" > /etc/nginx/conf.d/upstream.conf

RUN apt-get update
RUN apt-get install nano

CMD service nginx start
