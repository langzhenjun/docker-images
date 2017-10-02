FROM golang:alpine

RUN apk update && \
apk upgrade && \
apk add --no-cache git && \
go get github.com/langzhenjun/shadowsocks-go/cmd/shadowsocks-server && \
mkdir /shadowsocks-server

WORKDIR /shadowsocks-server
COPY *.json /shadowsocks-server/
EXPOSE 8080

ENTRYPOINT ["shadowsocks-server"]