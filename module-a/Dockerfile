FROM nginxinc/nginx-unprivileged:alpine
ENV NGINX_ENVSUBST_OUTPUT_DIR=/etc/nginx
COPY ./public /usr/share/nginx/html
COPY ./config /etc/nginx
EXPOSE 8081
