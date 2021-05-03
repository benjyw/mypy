python_library(
    sources=["**/*.pyi", "!@python2/**/*.pyi"],
    dependencies=[":versions"]
)

python_library(
    name="stdlib_py2",
    sources=["@python2/**/*.pyi"],
    dependencies=[":versions"]
)

resources(
    name="versions",
    sources=["VERSIONS"]
)
