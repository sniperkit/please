go_library(
    name = "parse",
    srcs = [
        "init.go",
        "parse_step.go",
        "rules.go",
        "suggest.go",
    ],
    visibility = ["PUBLIC"],
    deps = [
        "//src/core",
        "//src/fs",
        "//src/parse/asp",
        "//src/parse/rules",
        "//src/utils",
        "//third_party/go:gcfg",
        "//third_party/go:logging",
    ],
)

go_test(
    name = "parse_step_test",
    srcs = ["parse_step_test.go"],
    deps = [
        ":parse",
        "//src/core",
        "//third_party/go:testify",
    ],
)

go_test(
    name = "suggest_test",
    srcs = ["suggest_test.go"],
    deps = [
        ":parse",
        "//third_party/go:testify",
    ],
)

go_test(
    name = "rules_test",
    srcs = ["rules_test.go"],
    deps = [
        ":parse",
        "//third_party/go:testify",
    ],
)
