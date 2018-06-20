FROM redis:4.0.9-alpine
RUN mkdir /var/log/redis/ && chown redis:redis -R /var/log/redis/
COPY conf/redis.conf /usr/local/etc/redis/redis.conf

COPY entrypoint/docker-entrypoint.sh /entrypoint.sh
RUN chmod +x /entrypoint.sh
ENTRYPOINT ["/entrypoint.sh"]
CMD [ "redis-server", "/usr/local/etc/redis/redis.conf" ]