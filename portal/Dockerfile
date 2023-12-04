FROM nginxinc/nginx-unprivileged:alpine
ENV NGINX_ENVSUBST_OUTPUT_DIR=/etc/nginx

USER root
RUN mkdir /usr/share/nginx/cache
RUN chmod -R 777 /usr/share/nginx/cache

USER 101
COPY ./public /usr/share/nginx/html
COPY ./config /etc/nginx
EXPOSE 8080
