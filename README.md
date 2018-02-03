# Bazel Python

Experimenting using bazel to build a python project.

Sort of works.

```bash
brew install bazel
bazel build boom
bazel run boom
```

## Limitations

- Libraries pulled in from pip are not indexed for auto complete in Intellij
- Will it deal with non pure python packages?

## IntelliJ

- Install Python plugin
- Install Bazel plugin
- Import Bazel project selecting root dir as workspace
- Select the myview.bazelproject file




