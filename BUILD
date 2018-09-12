load("@com_github_grpc_grpc//bazel:cc_grpc_library.bzl", "cc_grpc_library")

cc_grpc_library(
    name = "foo_grpc",
    srcs = ["foo.proto"],
    proto_only = False,
    use_external = True,
    well_known_protos = False,
    deps = ["@com_google_protobuf//:timestamp_proto"],
)
