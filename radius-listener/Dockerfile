FROM golang:1.22
WORKDIR /usr/src/radius-listener

COPY . .

EXPOSE 8080

CMD ["./rcatcher", "--config", "config.ini"]
