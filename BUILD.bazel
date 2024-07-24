cc_library(
    name = "base64",
    srcs = ["base64.cpp"],
    hdrs = ["base64.h"],
    copts = [
        "-Werror",
        "-Wall",
        "-Wextra",
        "-pedantic",
        "-Wcast-align",
        "-Wcast-qual",
        "-Wctor-dtor-privacy",
        "-Wdisabled-optimization",
        "-Wformat=2",
        "-Winit-self",
        "-Wlogical-op",
        "-Wmissing-include-dirs",
        "-Wmissing-declarations",
        "-Wnoexcept",
        "-Wold-style-cast",
        "-Woverloaded-virtual",
        "-Wredundant-decls",
        "-Wshadow",
        "-Wsign-promo",
        "-Wstrict-null-sentinel",
        "-Wstrict-overflow=5",
        "-Wundef",
        "-Wno-unused",
        "-Wno-variadic-macros",
        "-Wno-parentheses",
        "-fdiagnostics-show-option",
    ],
)

cc_test(
    name = "base64_test_11",
    srcs = ["test.cpp"],
    deps = [":base64"],
    copts = ["-std=c++11"],
)

cc_test(
    name = "base64_test_17",
    srcs = ["test.cpp"],
    deps = [":base64"],
    copts = ["-std=c++17"],
)

test_suite(
    name = "all_tests",
    tests = [
        ":base64_test_11",
        ":base64_test_17",
    ],
)
