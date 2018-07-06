FROM alpine
RUN apk update && apk upgrade
RUN apk add php7 php7-json php7-iconv php7-phar php7-openssl
COPY rpg_service /app
EXPOSE 8080/tcp
EXPOSE 8080/udp
CMD cd /app; php -S localhost:8080 -t public public/index.php