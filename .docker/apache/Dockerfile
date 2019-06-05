FROM httpd:2.4.39-alpine
RUN apk update; apk upgrade;

COPY ezxss.apache.conf /usr/local/apache2/conf/ezxss.apache.conf
RUN echo "Include /usr/local/apache2/conf/ezxss.apache.conf" >> /usr/local/apache2/conf/httpd.conf
