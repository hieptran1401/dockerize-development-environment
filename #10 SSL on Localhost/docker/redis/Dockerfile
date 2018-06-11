FROM redis:4.0.9-alpine
RUN mkdir /var/log/redis/ && chown redis:redis -R /var/log/redis/
COPY redis.conf /usr/local/etc/redis/redis.conf
CMD [ "redis-server", "/usr/local/etc/redis/redis.conf" ]