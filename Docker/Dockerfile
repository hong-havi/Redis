FROM 7.2-rc-alpine3.17

# Add user
RUN addgroup -g 995 vboxsf
RUN addgroup redis vboxsf

COPY dockerfile/redis/redis.conf /etc/redis/redis.conf
RUN chown redis:redis /etc/redis/redis.conf

CMD ["redis-server", "/etc/redis/redis.conf"]