load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "json.go",
        "meta.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/ghodss/yaml:go_default_library",
        "//vendor/github.com/ugorji/go/codec:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/api/unversioned:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/runtime:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/runtime/serializer/recognizer:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/util/framer:go_default_library",
        "//vendor/k8s.io/client-go/1.5/pkg/util/yaml:go_default_library",
    ],
)
