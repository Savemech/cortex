load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "common.go",
        "doc.go",
    ],
    visibility = ["//visibility:public"],
    deps = ["//vendor/github.com/go-openapi/spec:go_default_library"],
)
