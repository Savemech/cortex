load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "idempotency.go",
        "unmarshal.go",
    ],
    visibility = ["//visibility:public"],
    deps = ["//vendor/github.com/aws/aws-sdk-go/aws/request:go_default_library"],
)

go_test(
    name = "go_default_xtest",
    srcs = [
        "idempotency_test.go",
        "protocol_test.go",
        "unmarshal_test.go",
    ],
    deps = [
        "//vendor/github.com/aws/aws-sdk-go/aws/client/metadata:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/aws/request:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/awstesting:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/ec2query:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/jsonrpc:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/query:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/rest:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/restjson:go_default_library",
        "//vendor/github.com/aws/aws-sdk-go/private/protocol/restxml:go_default_library",
        "//vendor/github.com/stretchr/testify/assert:go_default_library",
    ],
)
