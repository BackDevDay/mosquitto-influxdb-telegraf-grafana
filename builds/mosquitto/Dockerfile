FROM eclipse-mosquitto:1.6.12

RUN apk add --no-cache tzdata

COPY docker-entrypoint.sh /
ENTRYPOINT ["sh", "./docker-entrypoint.sh"]

CMD ["/usr/sbin/mosquitto", "-c", "/mosquitto/config/mosquitto.conf"]