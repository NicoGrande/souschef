load("@rules_python//python:defs.bzl", "py_library")

package(default_visibility = ["//visibility:public"])


py_library(
    name = "item",
    srcs = ["item.py"],
    deps = [
        ":quantity",
        ":nutritional_facts",
        "//src/utils:types", 
        "@pip//pydantic",
    ]
)

py_library(
    name = "quantity",
    srcs = ["quantity.py"],
    deps = [
        "//src/utils:types", 
        "@pip//pydantic",
    ]
)

py_library(
    name = "recipe",
    srcs = ["recipe.py"],
    deps = [
        ":item", 
        ":quantity", 
        ":nutritional_facts",
        "//src/utils:types", 
        "@pip//pydantic",
    ]
)

py_library(
    name = "receipt",
    srcs = ["receipt.py"],
    deps = [
        ":item", 
        ":quantity",
        "//src/utils:types", 
        "@pip//pydantic",
    ]
)

py_library(
    name = "nutritional_facts",
    srcs = ["nutritional_facts.py"],
    deps = [
        ":quantity",
        "//src/utils:types", 
        "@pip//pydantic",
    ]
)
