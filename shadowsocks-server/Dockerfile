FROM golang:alpine

RUN apk update && \
apk upgrade && \
apk add --no-cache git && \
go get github.com/langzhenjun/shadowsocks-go/cmd/shadowsocks-server

EXPOSE 8080

ENTRYPOINT ["shadowsocks-server"]