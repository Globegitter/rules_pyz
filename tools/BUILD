exports_files([
    "pip_generate-x64-linux",
    "pip_generate-x64-osx",
])

alias(
    name = "pip_generate",
    actual = select({
        "//rules_python_zip:linux": ":pip_generate-x64-linux",
        "//rules_python_zip:osx": ":pip_generate-x64-osx",
    }),
    visibility=["//visibility:public"],
)
