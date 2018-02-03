load("@foo//:requirements.bzl", "requirement")
load("@io_bazel_rules_docker//python:image.bzl", "py_image")

py_binary(
    name='boom',
    srcs=[
        'boom.py',
    ],
    deps=[
        requirement('tabulate')
    ]
)

py_image(
    name='boom-image',
    srcs=['boom.py'],
    main='boom.py',
)
