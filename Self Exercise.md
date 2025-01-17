```
docker run -d --name my-alpine alpine sleep 1000
```
```
docker inspect my-alpine
```
```
docker exec -it my-alpine sh
```
```
ls
```
```
exit
```

```
docker run -d --name my-nginx -p 8080:80 nginx
```
```
docker logs my-nginx
```
```
docker stats
```
```
docker stop my-nginx
```
```
docker rm my-nginx
```

```
docker pull nginx
```
```
docker run --name nginx-no-port -d nginx
```
```
docker ps
```
```
curl http://localhost
```
```
docker run --name nginx-with-port -d -p 8080:80 nginx
```
```
docker ps
```
```
docker inspect nginx-with-port | grep -i "port"
```
```
docker run --name nginx-port-8081 -d -p 8081:80 nginx
```
```
docker run --name nginx-port-8082 -d -p 8082:80 nginx
```
```
docker stop nginx-no-port nginx-with-port nginx-port-8081 nginx-port-8082
```
```
docker rm nginx-no-port nginx-with-port nginx-port-8081 nginx-port-8082
```
```
docker rmi nginx
```
