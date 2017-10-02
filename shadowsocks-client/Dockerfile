FROM golang:alpine

RUN apk update && \
apk upgrade && \
apk add --no-cache git && \
go get github.com/langzhenjun/shadowsocks-go/cmd/shadowsocks-local && \
mkdir /shadowsocks-local

WORKDIR /shadowsocks-local
COPY *.json $PWD/

EXPOSE 8081

ENTRYPOINT ["shadowsocks-local"]