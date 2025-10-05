# setup-kind

[![Current Tag](https://img.shields.io/github/v/tag/actionhippie/setup-kind?sort=semver)](https://github.com/actionhippie/setup-kind) [![Testing Build](https://github.com/actionhippie/setup-kind/workflows/testing/badge.svg)](https://github.com/actionhippie/setup-kind/actions/workflows/testing.yml)

[GitHub Action](https://github.com/features/actions) to install the
[Kind][kind] binary.

## Usage

```yml
name: Example

on:
  - push
  - pull_request

jobs:
  test:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v2

      - uses: actionhippie/setup-kind@v1

      - run: kind --help
```

## Inputs

### `version`

Version of the Kind binary

## Outputs

None

## Security

If you find a security issue please contact thomas@webhippie.de first.

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

* [Thomas Boerger](https://github.com/tboerger)

## License

Apache-2.0

## Copyright

```console
Copyright (c) 2024 Thomas Boerger <thomas@webhippie.de>
```

[kind]: https://kind.sigs.k8s.io/
