docker-oracle-xe-11g
============================
This is a fork of wnameless/oracle-xe-11g.  The only difference is that the password is `password`.  And the system time zone is new york.

Oracle Express Edition 11g Release 2 on Ubuntu 14.04.1 LTS

This **Dockerfile** is a [trusted build](https://registry.hub.docker.com/u/wnameless/oracle-xe-11g/) of [Docker Registry](https://registry.hub.docker.com/).

### Installation
```
docker pull guywithnose/oracle-xe-11g
```

Run with 22 and 1521 ports opened:
```
docker run -d -p 49160:22 -p 49161:1521 guywithnose/oracle-xe-11g
```

Connect database with following setting:
```
hostname: localhost
port: 49161
sid: xe
username: system
password: password
```

Password for SYS & SYSTEM
```
password
```

Login by SSH
```
ssh root@localhost -p 49160
password: admin
```
