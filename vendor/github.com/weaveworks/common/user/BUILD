load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "grpc.go",
        "http.go",
        "id.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/weaveworks/common/errors:go_default_library",
        "//vendor/golang.org/x/net/context:go_default_library",
        "//vendor/google.golang.org/grpc/metadata:go_default_library",
    ],
)
