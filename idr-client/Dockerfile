FROM golang:1.22
WORKDIR /usr/src/idr-client

COPY . .

RUN ls -l

EXPOSE 8080

CMD ["./idrclient", "--config", "config.ini"]
