load("@io_bazel_rules_go//go:def.bzl", "go_binary", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["main.go"],
    visibility = ["//visibility:private"],
    deps = [
        "//pkg/chunk:go_default_library",
        "//pkg/distributor:go_default_library",
        "//pkg/querier:go_default_library",
        "//pkg/ring:go_default_library",
        "//pkg/util:go_default_library",
        "//vendor/github.com/prometheus/client_golang/prometheus:go_default_library",
        "//vendor/github.com/prometheus/common/log:go_default_library",
        "//vendor/github.com/prometheus/common/route:go_default_library",
        "//vendor/github.com/prometheus/prometheus/promql:go_default_library",
        "//vendor/github.com/prometheus/prometheus/retrieval:go_default_library",
        "//vendor/github.com/prometheus/prometheus/web/api/v1:go_default_library",
        "//vendor/github.com/weaveworks/common/middleware:go_default_library",
        "//vendor/github.com/weaveworks/common/server:go_default_library",
        "//vendor/golang.org/x/net/context:go_default_library",
        "//vendor/google.golang.org/grpc:go_default_library",
    ],
)

go_binary(
    name = "querier",
    library = ":go_default_library",
    visibility = ["//visibility:public"],
)
