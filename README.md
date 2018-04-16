# Zabbix 3.5


```bash
docker build -f build-mariadb/Dockerfile -t registry.d2d.com.br:5000/mariadb:1.0.0 .
docker build -f build-zabbix/Dockerfile -t registry.d2d.com.br:5000/zabbix:1.0.0 .
```

```bash
docker volume create --name=mysql
docker volume create --name=zabbix
```

docker-compose up -d
docker exec -it mariadb ./script.sh
