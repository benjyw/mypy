
python_library(
    dependencies=[
        "//:types-mypy-extensions",
        "//:types-typing-extensions",
        "//:types-typed-ast",
        "//:types-toml",
        "//:types-enum34",
        "mypy/xml",
    ]
)

python_library(
    name="py3",
    sources=[],
    dependencies=[
        ":mypy",
        "mypy/typeshed/stdlib",
    ],
    interpreter_constraints=[">=3.7"],
)

python_library(
    name="py2",
    sources=[],
    dependencies=[
        ":mypy",
        "mypy/typeshed/stdlib:stdlib_py2",
    ]
)

pex_binary(
    name="bin",
    dependencies=[
        ":py2",
        ":py3",
        "mypy/__main__.py",
        "//:importlib-metadata",
        "//:pytest",
    ],
    entry_point="mypy",
    execution_mode="venv",
)
