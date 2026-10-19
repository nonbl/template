<!--
SPDX-FileCopyrightText: 2026 Crown Orange, Bulgaria
SPDX-License-Identifier: Apache-2.0
-->

# PROJECT_NAME

[![CI](https://github.com/nonbl/PROJECT_NAME/actions/workflows/ci.yml/badge.svg)](https://github.com/nonbl/PROJECT_NAME/actions/workflows/ci.yml)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache--2.0-blue.svg)](LICENSES/Apache-2.0.txt)
[![REUSE compliant](https://img.shields.io/badge/REUSE-compliant-green.svg)](https://reuse.software/)

Nonbl® is a registered trademark of Crown Orange EOOD, Bulgaria.

`PROJECT_NAME` is PROJECT_DESCRIPTION for the **Nonbl** automation platform.

> **Using this template:** replace `PROJECT_NAME` and `PROJECT_DESCRIPTION` in
> `README.md`, `NOTICE`, `CONTRIBUTING.md` and `SECURITY.md`; add third-party
> attributions to `NOTICE` if the project carries any; then delete this note.

## Requirements

- C++23 compiler (GCC, Clang, or MSVC)
- CMake 3.22+

## Building

```bash
cmake -B build -DCMAKE_BUILD_TYPE=Debug
cmake --build build -j$(nproc)
```

### Running tests

```bash
cd build && ctest -j$(nproc) --output-on-failure
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## Security

Do not open public issues for security vulnerabilities. Email
**security@nonbl.com** — see [SECURITY.md](SECURITY.md) for the disclosure
policy and response timelines.

## License

Licensed under the [Apache License 2.0](LICENSES/Apache-2.0.txt).
Test data fixtures and the tool-configuration dotfiles (`.clang-format`,
`.cmake-format`, `.gitattributes`, `.gitignore`, `REUSE.toml`) are released
under [CC0-1.0](LICENSES/CC0-1.0.txt).

See [NOTICE](NOTICE) for attribution.
