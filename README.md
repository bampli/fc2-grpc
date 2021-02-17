# gRPC & protocol-buffers

## Get Started

### Go

https://golang.org/doc/install?download=go1.16.linux-amd64.tar.gz

### Protobuf

    sudo apt update
    sudo apt install protobuf-compiler

### Modules

    go get -u google.golang.org/grpc
    go install google.golang.org/grpc

    go get -u google.golang.org/protobuf/cmd/protoc-gen-go
    go install google.golang.org/protobuf/cmd/protoc-gen-go

    go get -u google.golang.org/grpc/cmd/protoc-gen-go-grpc
    go install google.golang.org/grpc/cmd/protoc-gen-go-grpc

### Compile

    protoc --proto_path=proto proto/*.proto --go_out=pb --go-grpc_out=pb

### gRPC client

    sudo curl -L 'https://github.com/ktr0731/evans/releases/download/0.9.3/evans_linux_amd64.tar.gz' | tar xvzf -
    file evans
    sudo mv evans /usr/local/bin/evans

    evans -r repl --host localhost --port 50051

