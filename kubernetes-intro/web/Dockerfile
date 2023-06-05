FROM nginx
RUN usermod -u 1001 nginx
COPY default.conf /etc/nginx/conf.d/
WORKDIR /app
EXPOSE 8000
