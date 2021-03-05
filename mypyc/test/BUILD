python_library()

python_requirement_library(
    name="six",
    requirements=["six==1.15.0"]
)

python_tests(
    name="tests",
    dependencies=[
        ":six",
        "//:virtualenv",
        "scripts:mypyc",
        "test-data",
        "mypy/__main__.py",
        "mypy/dmypy/__main__.py",
        "mypy/test/data.py",
        "mypyc/build.py",
        "mypyc/external/googletest",
        "mypyc/lib-rt",
        "mypyc/test-data",
    ],
)
