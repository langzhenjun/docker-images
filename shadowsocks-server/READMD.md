# Shadowsocks Server

## build docker image
```bash
docker build -t shadowsocks-server .
```

## run docker container
1. default
```bash
docker run --name shadowsocks-server -p 8080:8080 shadowsocks-server -c configs.default.json
```

2. multiple ports
```bash
docker run --name shadowsocks-server -p 8080:8080 shadowsocks-server -c configs.mutiple.ports.json
```