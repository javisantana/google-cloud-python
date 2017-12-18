# Changelog

[PyPI History][1]

[1]: https://pypi.org/project/google-cloud-vision/#history

## 0.29.0

### :warning: Breaking Changes

- The HTTP/JSON based client that was deprecated in 0.25.0 is completely
  removed.

### Release Candidate

- This is the (hopefully) final release candidate before declaring a stable
  release.

### Features

- The `v1p1beta1` endpoint has been added. (#4493)

  This is a superset of `v1` and includes features that are still in beta
  on the API side. You can opt in to this endpoint by importing it explicitly:

  ```python
  from google.cloud import vision_v1p1beta1
  client = vision_v1p1beta1.ImageAnnotatorClient()
  ```

PyPI: https://pypi.org/project/google-cloud-vision/0.29.0/


## 0.28.0

### Notable Implementation Changes

- Update and re-organize autogenerated code (#3952)

### Documentation

- Added link to "Python Development Environment Setup Guide" in
  project README (#4187, h/t to @michaelawyu)

### Dependencies

- Upgrading to `google-cloud-core >= 0.28.0` and adding dependency
  on `google-api-core` (#4221, #4280)
- Deferring to `google-api-core` for `grpcio` and
  `googleapis-common-protos`dependencies (#4096, #4098)

PyPI: https://pypi.org/project/google-cloud-vision/0.28.0/