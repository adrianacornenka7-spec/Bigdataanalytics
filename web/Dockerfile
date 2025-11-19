FROM ubuntu
RUN apt-get update
RUN apt-get install -y golang
COPY . /
RUN go build -o dispatcher dispatcher.go
CMD ["./dispatcher"]

