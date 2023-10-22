FROM golang:1.19
WORKDIR /app
COPY ./main.go .
RUN go mod init tidy
RUN go mod tidy
RUN go get .
RUN go build -o main .
CMD ["./main"] 
