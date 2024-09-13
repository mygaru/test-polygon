FROM golang:1.22
WORKDIR /usr/src/radius-listener

COPY . .

EXPOSE 80 443

CMD ["./rcatcher", "--config", "config.ini"]
