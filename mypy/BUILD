
python_library(
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
    name="bin",
    dependencies=[
        "mypy/__main__.py",
    ],
    entry_point="mypy",
    execution_mode="venv",
    interpreter_constraints=[">=3.7"],
)
