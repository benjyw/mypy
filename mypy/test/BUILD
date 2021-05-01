python_library(
    sources=["*.py", "!test*.py"]
)

python_tests(
    name="tests",
    sources=["test*.py"],
    dependencies=[
        "//:importlib-metadata",
        "//:pytest",
        "test-data",
        "mypy/__main__.py",
        "mypy/dmypy/__main__.py",
        "mypy/test/data.py"
    ],
)
