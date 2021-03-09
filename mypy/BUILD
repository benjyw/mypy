
python_library(
    dependencies=[
        "//:types-mypy-extensions",
        "//:types-typing-extensions",
        "mypy/xml",
    ]
)

python_library(
    name="py3",
    sources=[],
    dependencies=[
        ":mypy",
        "mypy/typeshed/stdlib",
    ]
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
        ":py3",
        "mypy/__main__.py",
    ],
    entry_point="mypy"
)
