load(
    "//bazel:envoy_build_system.bzl",
    "envoy_cc_library",
    "envoy_package",
)

envoy_package()

envoy_cc_library(
    name = "config_schemas_lib",
    srcs = ["config_schemas.cc"],
    hdrs = ["config_schemas.h"],
)

envoy_cc_library(
    name = "json_loader_lib",
    srcs = ["json_loader.cc"],
    hdrs = ["json_loader.h"],
    external_deps = ["rapidjson"],
    deps = ["//include/envoy/json:json_object_interface"],
)

envoy_cc_library(
    name = "json_validator_lib",
    hdrs = ["json_validator.h"],
    deps = ["//include/envoy/json:json_object_interface"],
)
