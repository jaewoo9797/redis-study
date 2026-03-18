# 02 레디스 시작하기

```
docker ps
CONTAINER ID   IMAGE                       COMMAND                   CREATED         STATUS         PORTS                                         NAMES
03b77a04ad79   redis-redis-master          "docker-entrypoint.s…"   6 seconds ago   Up 6 seconds   0.0.0.0:6379->6379/tcp, [::]:6379->6379/tcp   study-redis
```

docker 컨테이너 접속 명령어

```
docker exec -it <container-name> redis-cli
127.0.0.1:6379>
```

## 데이터 저장과 조회

```
> SET hello world
OK
```

레디스는 key-value 스토어이며, 위의 커맨드는 hello라는 key에 world 라는 값을 저장하는 것을 나타낸다.

```
> GET hello
"world"
```
