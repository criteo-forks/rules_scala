load("//scala:scala.bzl", "scala_binary", "scala_library")

scala_library(
  name = "tut_compiler_lib",
  srcs = ["TutCompiler.scala"],
  deps = [
    "//external:io_bazel_rules_scala/dependency/tut/tut_core",
    "//src/scala:scala_compiler",
    "//src/java/io/bazel/rulesscala/io_utils",
  ],
  visibility = ["//visibility:public"],
)

scala_binary(
  name = "tut_compiler",
  main_class = "io.bazel.rules_scala.tut_support.TutCompiler",
  deps = [":tut_compiler_lib"],
  visibility = ["//visibility:public"],
)
