FROM openresty/openresty:alpine

LABEL version 1.0.0
COPY nginx.conf         /usr/local/openresty/nginx/conf/
COPY *.vhost            /usr/local/openresty/nginx/conf/
COPY lib/prometheus.lua /usr/local/openresty/luajit/lib

EXPOSE 80
EXPOSE 32111

RUN nginx -t