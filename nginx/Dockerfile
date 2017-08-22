FROM nginx:alpine
RUN rm /etc/nginx/conf.d/default.conf
ADD conf/nginx.conf /etc/nginx/nginx.conf
ADD conf.d/my.conf /etc/nginx/conf.d/my.conf
