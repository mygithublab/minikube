package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["interface.go"],
    deps = [
        "//pkg/client/informers/informers_generated/internalversion/internalinterfaces:go_default_library",
        "//pkg/client/informers/informers_generated/internalversion/networking/internalversion:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//pkg/client/informers/informers_generated/internalversion/networking/internalversion:all-srcs",
    ],
    tags = ["automanaged"],
)
