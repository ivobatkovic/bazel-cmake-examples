cc_library(
    name = "boost-headers",
    deps =  select({
            "@platforms//os:osx" : [ "@boost_osx//:boost-headers"],
            "//conditions:default" : ["@boost_linux//:boost-headers"],
    }),
    visibility = ["//visibility:public"],
)

cc_library(
    name = "boost-regex",
    deps =  select({
            "@platforms//os:osx" : [ "@boost_osx//:boost-regex"],
            "//conditions:default" : ["@boost_linux//:boost-regex"],
    }),
    visibility = ["//visibility:public"],
)
