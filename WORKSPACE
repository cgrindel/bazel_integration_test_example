workspace(name = "cgrindel_bazel_integration_test_example")

http_archive(
    name = "cgrindel_rules_bazel_integration_test",
    sha256 = "4fa679d98318df3e280e9c8b7f445cd06de7954aa0454702a62ebab8c820ce7e",
    strip_prefix = "rules_bazel_integration_test-0.1.0",
    urls = ["https://github.com/cgrindel/rules_bazel_integration_test/archive/v0.1.0.tar.gz"],
)

load("@cgrindel_rules_bazel_integration_test//bazel_integration_test:deps.bzl", "bazel_integration_test_rules_dependencies")

bazel_integration_test_rules_dependencies()

load("@bazel_skylib//:workspace.bzl", "bazel_skylib_workspace")

bazel_skylib_workspace()

load("@cgrindel_rules_bzlformat//bzlformat:deps.bzl", "bzlformat_rules_dependencies")

bzlformat_rules_dependencies()

load("@cgrindel_bazel_starlib//:deps.bzl", "bazel_starlib_dependencies")

bazel_starlib_dependencies()

load("//:bazel_versions.bzl", "SUPPORTED_BAZEL_VERSIONS")
load("@build_bazel_integration_testing//tools:repositories.bzl", "bazel_binaries")

bazel_binaries(versions = SUPPORTED_BAZEL_VERSIONS)
