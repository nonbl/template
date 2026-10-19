<!--
SPDX-FileCopyrightText: 2026 Crown Orange, Bulgaria
SPDX-License-Identifier: Apache-2.0
-->

# Contributing to PROJECT_NAME

Thanks for your interest in improving `PROJECT_NAME`. It is part of the
**nonbl** platform — please read this guide before opening a pull request.

## Development setup

Requirements: a C++23 compiler (GCC, Clang, or MSVC) and CMake 3.22+.

```bash
# Configure
cmake -B build -DCMAKE_BUILD_TYPE=Debug

# Build
cmake --build build -j$(nproc)

# Test
cd build && ctest -j$(nproc) --output-on-failure
```

## Before you open a pull request

1. **Add or update tests.** New behaviour needs coverage; bug fixes need a
   regression test. The suite must stay green.
2. **Format your code.** Run `clang-format -i` on every changed C/C++ file
   (the repository ships a `.clang-format`). CMake files follow `.cmake-format`.
3. **Build warning-clean.** CI compiles with warnings as errors; keep the
   build free of warnings under `-Wall -Wextra -Wconversion`.
4. **Keep licensing intact.** The repository is
   [REUSE](https://reuse.software)-compliant; `reuse lint` must pass. Every
   new source file needs an SPDX header — an `SPDX-License-Identifier` tag set
   to `Apache-2.0`, plus at least one copyright (`SPDX-FileCopyrightText`)
   line. You keep the copyright to your contribution: use your own (or your
   employer's) name and year. SPDX supports multiple copyright holders per
   file, so add yours rather than replacing existing lines. Contributions are
   accepted under the project's Apache-2.0 license (inbound = outbound).
5. **Mind wire compatibility.** Changing the order, size, or meaning of a wire
   field is a breaking change. Prefer additive, optional tail fields.

## Commit messages

Write clear, imperative commit messages that explain the change and its
rationale.

## Code of conduct

Participation in this project is governed by our
[Code of Conduct](CODE_OF_CONDUCT.md).

## Reporting security issues

Do **not** open public issues for security vulnerabilities. Follow the process
in [SECURITY.md](SECURITY.md).
