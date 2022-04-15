# bazel_python_repo

This repo demonstrates how to setup a python monorepo.
All python projects will exist under a common namespace "acme_corp".


Run app1:
```
bazel run python_projects/acme_corp/app1:app1_module1
```

Create app1 binary:
```
bazel build python_projects/acme_corp/app1:app1_module1
```

Run binary directly:
```
bazel-bin/python_projects/acme_corp/app1/app1_module1
```

Run lib1 tests:
```
bazel test python_projects/acme_corp/lib1/tests/unit:unit
```

Run all tests:
```
bazel test python_projects/...
```

Create sdist of lib1:
```
bazel build python_projects/acme_corp/lib1:create_dist
```

The resulting artifact can be found at `bazel-bin/python_projects/acme_corp/lib1/acme_corp.lib.tar.gz`

