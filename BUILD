load("@com_github_grpc_grpc//bazel:cc_grpc_library.bzl", "cc_grpc_library")

# Works:
proto_library(
    name = "foo_proto",
    srcs = ["foo.proto"],
    deps = ["@com_google_protobuf//:timestamp_proto"],
)

# Works:
cc_proto_library(
    name = "foo_cc_proto",
    deps = [":foo_proto"],
)

# Works:
cc_grpc_library(
    name = "foo_cc_grpc",
    srcs = [":foo_proto"],
    deps = [":foo_cc_proto"],
    grpc_only = True,
)
