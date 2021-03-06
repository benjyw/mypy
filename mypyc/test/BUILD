python_library()

python_requirement_library(
    name="six",
    requirements=["six==1.15.0"]
)

# This file is named test_serialization.py even though it doesn't
# contain its own tests so that pytest will rewrite the asserts...
python_library(
    name="test_serialization",
    sources=["test_serialization.py"],
)

python_tests(
    name="tests",
    sources=["test_*.py", "!test_serialization.py"],
    dependencies=[
        ":six",
        ":test_serialization",
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
