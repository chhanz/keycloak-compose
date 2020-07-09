# keycloak-compose
Keycloak + pgsql 서비스 운영 환경을 위한 Compose File 입니다.   
# Compose 설치
## Podman-compose 설치
```bash
curl -o /usr/local/bin/podman-compose https://raw.githubusercontent.com/containers/podman-compose/devel/podman_compose.py
chmod +x /usr/local/bin/podman-compose
```
## Docker-compose 설치
```bash
curl -L "https://github.com/docker/compose/releases/download/1.26.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose
```
# Volume 설정
`/root/sqldata` (default) 경로 생성 필요.   
   
# 서비스 시작
```bash
$ docker-compose up -d
```
or   
```bash
$ podman-compose up -d 
```
   
# 서비스 중지
```bash
$ docker-compose stop -d
```
or   
```bash
$ podman-compose stop -d 
```
  