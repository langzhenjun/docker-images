# Shadowsocks Client

## build docker image
```bash
docker build -t shadowsocks-client .
```

## run docker container
1. default
```bash
docker run --name shadowsocks-client -p 8081:8081 shadowsocks-client -c configs.defualt.json
```

2. multiple servers
```bash
docker run --name shadowsocks-client -p 8081:8081 shadowsocks-client -c configs.multiple.server.json
```