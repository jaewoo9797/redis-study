FROM redis:latest

# local redis.conf를 컨테이너 내부로 복사
COPY redis.conf /usr/local/etc/redis/redis.conf

CMD ["redis-server", "/usr/local/etc/redis/redis.conf"]