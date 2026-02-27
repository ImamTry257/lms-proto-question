# Question Proto


## How to generate file question.proto
protoc --proto_path=proto/question --go_out=gen/go/question --go_opt=paths=source_relative --go-grpc_out=gen/go/question --go-grpc_opt=paths=source_relative proto/question/question.proto

when error get package, use it
go env -w GOPRIVATE=gitlab.com/bykarya-proto/* && go env -w GONOSUMDB=gitlab.com/bykarya-proto/* && go env -w GONOPROXY=gitlab.com/bykarya-proto/*
##
