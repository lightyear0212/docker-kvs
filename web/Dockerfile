From nginx:1.17.5-alpine
COPY ./start.sh /usr/local/bin/start.sh
RUN chmod +x /usr/local/bin/start.sh
COPY ./nginx.tpl /etc/nginx/nginx.tpl
COPY ./html/ /usr/share/nginx/html/
ENV PORT 80
ENV APP_SERVER "http://192.168.3.16:8080"
CMD ["/usr/local/bin/start.sh"]