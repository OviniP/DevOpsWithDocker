#Backend
FROM golang:1.16

WORKDIR /app
COPY . .

RUN go build
RUN go test ./....

CMD ["go", "run", "server"]