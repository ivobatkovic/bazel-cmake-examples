
cc_library(
    name = "boost-filesystem",
    deps =  select({
            "@platforms//os:osx" : [ "@boost_osx//:boost-filesystem"],
            "//conditions:default" : ["@boost_linux//:boost-filesystem"],
    }),
    visibility = ["//visibility:public"],
)
