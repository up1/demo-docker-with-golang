FROM golang:1.11.2-alpine3.8
WORKDIR /xxx
COPY . .
RUN CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo -o app .
CMD ["./app"]