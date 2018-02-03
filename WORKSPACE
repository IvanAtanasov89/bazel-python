git_repository(
    name = "io_bazel_rules_python",
    remote = "https://github.com/bazelbuild/rules_python.git",
    commit = "73a154a181a53ee9e021668918f8a5bfacbf3b43",
)

git_repository(
    name = "io_bazel_rules_docker",
    remote = "https://github.com/bazelbuild/rules_docker.git",
    tag = "v0.3.0"
)

load("@io_bazel_rules_python//python:pip.bzl", "pip_import")

pip_import(
    name = "foo",
    requirements = "//boom:requirements.txt",
)
load("@foo//:requirements.bzl", "pip_install")
pip_install()

load(
    "@io_bazel_rules_docker//python:image.bzl",
    _py_image_repos = "repositories",
)

_py_image_repos()
