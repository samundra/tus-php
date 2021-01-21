FROM tus-php-base

COPY ./configs/default.conf /etc/nginx/conf.d/default.conf

EXPOSE 80
#ENV SERVER_URL http://0.0.0.0:8081
ENV SERVER_URL https://e4063466d30b.ngrok.io

WORKDIR /var/www/html

ENTRYPOINT ["/usr/bin/supervisord", "-n", "-c",  "/etc/supervisord.conf"]
