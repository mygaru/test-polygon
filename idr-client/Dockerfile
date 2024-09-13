FROM golang:1.22
WORKDIR /usr/src/idr-client

COPY . .

RUN ls -l

EXPOSE 80 443

CMD ["idrclient", "-config", "config.ini"]
