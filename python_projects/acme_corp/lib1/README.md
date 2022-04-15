# acme_corp.lib1

## Build sdist

Run this from this directory:
```
bazel build :create_dist
```

Artifact will be available at `bazel-bin/python_projects/acme_corp/lib1/acme_corp.lib.tar.gz`

## Run tests

```
bazel test tests/unit
```
