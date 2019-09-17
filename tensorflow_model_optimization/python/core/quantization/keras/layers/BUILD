package(default_visibility = [
    "//tensorflow_model_optimization:__subpackages__",
])

licenses(["notice"])  # Apache 2.0

py_library(
    name = "conv_batchnorm",
    srcs = ["conv_batchnorm.py"],
    srcs_version = "PY2AND3",
    deps = [
        # python:array_ops tensorflow dep2,
        # python:math_ops tensorflow dep2,
        # python:nn tensorflow dep2,
        # python:nn_ops tensorflow dep2,
        # python/keras:backend tensorflow dep2,
        # python/keras:engine_utils tensorflow dep2,
        # python/keras:layers_base tensorflow dep2,
    ],
)

py_test(
    name = "conv_batchnorm_test",
    srcs = ["conv_batchnorm_test.py"],
    deps = [
        ":conv_batchnorm",
        # tensorflow dep1,
        "//tensorflow_model_optimization/python/core/quantization/keras:utils",
    ],
)