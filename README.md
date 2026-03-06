# Learning Proto


## How to generate file learning.proto
protoc --proto_path=proto/learning --go_out=gen/go/learning --go_opt=paths=source_relative --go-grpc_out=gen/go/learning --go-grpc_opt=paths=source_relative proto/learning/learning.proto

when error get package, use it
go env -w GOPRIVATE=gitlab.com/bykarya-proto/* && go env -w GONOSUMDB=gitlab.com/bykarya-proto/* && go env -w GONOPROXY=gitlab.com/bykarya-proto/*
##
