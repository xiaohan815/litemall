FROM nginx
VOLUME /tmp
ENV LANG en_US.UTF-8
COPY dist /data
RUN rm /etc/nginx/conf.d/*.conf && rm /etc/nginx/nginx.conf
ADD nginx.conf /etc/nginx/
ADD default.conf /etc/nginx/conf.d/
EXPOSE 80
RUN /bin/bash -c 'echo init admin nginx ok'
