```
$ bazel build :foo_grpc
Starting local Bazel server and connecting to it...
INFO: SHA256 (https://github.com/grpc/grpc/archive/master.tar.gz) = a986d6e1ffcd743a2bcdfd1c573458d3192fb47617454112b75f1ea7482db477
INFO: SHA256 (https://github.com/google/protobuf/archive/48cb18e5c419ddd23d9badcfe4e9df7bde1979b2.tar.gz) = f5a35e17fb07f3b13517264cd17a089636fcbb2912f9df7bef7414058969a8d2
ERROR: HOME/opencensus/timestamp_proto/BUILD:3:1: no such target '@com_google_protobuf//:_timestamp_proto_only': target '_timestamp_proto_only' not declared in package '' defined by HOME/.cache/bazel/_bazel_easy/fc37c12b1419c01ea4f7e1e2af842623/external/com_google_protobuf/BUILD and referenced by '//:_foo_grpc_only'
ERROR: Analysis of target '//:foo_grpc' failed; build aborted: Analysis failed
INFO: Elapsed time: 19.938s
INFO: 0 processes.
FAILED: Build did NOT complete successfully (9 packages loaded)
```
