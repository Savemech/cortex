load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "error.go",
        "ini.go",
        "key.go",
        "parser.go",
        "section.go",
        "struct.go",
    ],
    visibility = ["//visibility:public"],
)

go_test(
    name = "go_default_test",
    srcs = [
        "ini_test.go",
        "key_test.go",
        "parser_test.go",
        "section_test.go",
        "struct_test.go",
    ],
    library = ":go_default_library",
    deps = ["//vendor/github.com/smartystreets/goconvey/convey:go_default_library"],
)
