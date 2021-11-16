# Example Demonstrating Usage for `rules_bazel_integration_test`

[![Build](https://github.com/cgrindel/rules_bazel_integration_test/actions/workflows/bazel.yml/badge.svg)](https://github.com/cgrindel/rules_bazel_integration_test/actions/workflows/bazel.yml)

Minimal example demonstrating the use of
[rules_bazel_integration_test](https://github.com/cgrindel/rules_bazel_integration_test).

The parent repository has no functionality of its own. It exists to show the minimum configuration
to use `rules_bazel_integration_test`. The [examples/simple](/examples/simple) workspace is a toy
project which has some tests.

The integration tests can be executed by running the following:

```sh
# Execute all of the integration tests
$ bazel test //examples:all_integration_tests
```


