load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = [
        "connection.go",
        "connection_maker.go",
        "gossip.go",
        "gossip_channel.go",
        "local_peer.go",
        "logger.go",
        "overlay.go",
        "peer.go",
        "peer_name_mac.go",
        "peers.go",
        "protocol.go",
        "protocol_crypto.go",
        "router.go",
        "routes.go",
        "status.go",
        "surrogate_gossiper.go",
        "token_bucket.go",
    ],
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/golang.org/x/crypto/nacl/box:go_default_library",
        "//vendor/golang.org/x/crypto/nacl/secretbox:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "gossip_test.go",
        "mocks_test.go",
        "peer_test.go",
        "peers_test.go",
        "protocol_test.go",
        "surrogate_gossiper_test.go",
    ],
    library = ":go_default_library",
    deps = ["//vendor/github.com/stretchr/testify/require:go_default_library"],
)

go_test(
    name = "go_default_xtest",
    srcs = [
        "peer_name_mac_test.go",
        "protocol_crypto_test.go",
        "routes_test.go",
        "token_bucket_test.go",
    ],
    deps = [
        "//vendor/github.com/stretchr/testify/require:go_default_library",
        "//vendor/github.com/weaveworks/mesh:go_default_library",
    ],
)
