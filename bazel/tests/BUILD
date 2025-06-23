load("@bazel_skylib//:bzl_library.bzl", "bzl_library")
load(":java_proto_library_tests.bzl", "java_proto_library_test_suite")
load(":proto_common_check_collocated_tests.bzl", "proto_common_check_collocated_test_suite")
load(":proto_common_compile_tests.bzl", "proto_common_compile_test_suite")
load(":proto_common_declare_generated_files_tests.bzl", "proto_common_declare_generated_files_test_suite")
load(":proto_common_should_generate_tests.bzl", "proto_common_should_generate_test_suite")

package(default_applicable_licenses = ["//:license"])

proto_common_compile_test_suite(name = "proto_common_compile_test_suite")

proto_common_should_generate_test_suite(name = "proto_common_should_generate_test_suite")

proto_common_declare_generated_files_test_suite(name = "proto_common_declare_generated_files_test_suite")

proto_common_check_collocated_test_suite(name = "proto_common_check_collocated_test_suite")

java_proto_library_test_suite(name = "java_proto_library_test_suite")

bzl_library(
    name = "protobuf_test_proto_library_bzl",
    srcs = ["protobuf_test_proto_library.bzl"],
    parse_tests = False,
    visibility = ["//visibility:private"],
)
