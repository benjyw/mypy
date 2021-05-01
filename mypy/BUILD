
python_library(
    name="lib",
    dependencies=[
        "//:typing-extensions",
        "//:types-mypy-extensions",
        "//:types-typed-ast",
        "//:types-toml",
        "//:types-enum34",
        "mypy/xml",
        "mypy/typeshed/stdlib",
        "mypy/typeshed/stdlib:stdlib_py2",
    ],
)

pex_binary(
    name="mypy",
    dependencies=[
        ":lib",
    ],
    entry_point="mypy",
    execution_mode="venv",
)
