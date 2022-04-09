load("@rules_cc//cc:defs.bzl", "cc_binary", "cc_library", "cc_test")

cc_library(
    name = "foo",
    srcs = ["foo.cpp"],
    hdrs = ["foo.h"],
)

cc_test(
    name = "foo_test",
    srcs = ["foo_test.cpp"],
    deps = [
        ":foo",
        "@googletest//:gtest",
        "@googletest//:gtest_main",
    ],
)

cc_binary(
    name = "main",
    srcs = ["main.cpp"],
    deps = [":foo"],
)
