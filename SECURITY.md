<!--
SPDX-FileCopyrightText: 2026 Crown Orange, Bulgaria
SPDX-License-Identifier: Apache-2.0
-->

# Security Policy

If you believe you have found a security vulnerability in Nonbl, please report
it privately. **Do not open a public issue or pull request for security
vulnerabilities** — public disclosure before a fix is available puts other
users at risk.

## Reporting a vulnerability

Use GitHub's private vulnerability reporting: open the **Security** tab of
this repository and choose **Report a vulnerability**. The report is visible
only to the maintainers, and it is the channel we watch first.

If you would rather not use GitHub, email **security@nonbl.com**.

Either way, please include:

- A description of the issue and the component(s) affected (e.g. the
  public API, a decoder, or a validator)
- Steps to reproduce, or a proof-of-concept if you have one
- The version, commit hash, or deployment where you observed the issue
- Your assessment of the impact, if you have one
- Whether you would like credit in the disclosure

## What to expect

- **Acknowledgement within 2 business days.** We confirm receipt and assign a
  tracking identifier.
- **Initial severity assessment within 5 business days.** We share our
  classification (critical / high / medium / low) and expected next steps with
  the reporter.
- **Fix timeline depends on severity.** Critical issues are prioritised
  immediately; lower-severity issues are scheduled into the regular release
  cycle. We keep the reporter informed throughout.
- **Coordinated disclosure.** We ask that reporters hold public disclosure
  until a fix is available or until we have agreed a disclosure date. We are
  happy to credit reporters in the advisory unless they prefer to remain
  anonymous.

## Scope

This policy covers **PROJECT_NAME**, the project in this repository.

Third-party dependencies are out of scope; please report those to the
respective upstream project. Vulnerabilities in other Nonbl components should be
reported through that component's own security policy. If you are unsure where
an issue belongs, email us anyway and we will route it.

## Safe harbour

We will not pursue legal action against researchers who:

- Make a good-faith effort to avoid privacy violations, data destruction, and
  service disruption
- Report the issue to us privately and give us reasonable time to respond
  before any public disclosure
- Do not access, modify, or retain data belonging to other users beyond what
  is strictly necessary to demonstrate the issue
