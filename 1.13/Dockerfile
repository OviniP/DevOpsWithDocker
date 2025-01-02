FROM golang:1.16
ENV PORT 8081
EXPOSE 8081

WORKDIR /app
COPY . .

RUN go build
RUN go test ./....

CMD ["go", "run", "server"]