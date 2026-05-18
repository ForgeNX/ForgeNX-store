FROM golang:1.22-alpine

WORKDIR /app

RUN apk add --no-cache git

RUN git clone https://github.com/ForgeNX/forgenx-engine.git .

RUN go build -o forgenx-engine ./cmd/gostratumengine

EXPOSE 3333
EXPOSE 8080

CMD ["./forgenx-engine"]
