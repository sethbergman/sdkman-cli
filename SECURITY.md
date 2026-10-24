# Security Policy

Thank you for helping keep SDKMAN! and its users safe. This document describes how to report security vulnerabilities in the SDKMAN! CLI and what you can expect from the maintainers in return.

**Note:** SDKMAN! CLI is in maintenance mode. The shell-based commands are being rewritten in Rust in the [sdkman-cli-native](https://github.com/sdkman/sdkman-cli-native) project, which maintains its own security policy. Please report each issue to the repository that corresponds to the affected code.

## Supported Versions

Only the latest released version of SDKMAN! CLI receives security updates. Because SDKMAN! offers self-updates, users are expected to be running a recent release.

| Version | Supported |
| ------- | --------- |
| Latest  | ✅        |
| Older   | ❌        |

The same policy applies to [sdkman-cli-native](https://github.com/sdkman/sdkman-cli-native): only the latest release is supported.

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub issues, Discord, or any other public channel.**

There are two ways to report a vulnerability privately:

1. **GitHub Private Vulnerability Reporting (preferred):** open a report at <https://github.com/sdkman/sdkman-cli/security/advisories/new>.
2. **Email (fallback):** send a report to [security@sdkman.io](mailto:security@sdkman.io).

Please include as much of the following as you can:

- A description of the issue and the impact you believe it has
- Steps to reproduce, including affected command(s), shell, and OS
- The SDKMAN! CLI version (`sdk version`) and Java version where relevant
- Any proof-of-concept code, logs, or screenshots
- Your name and contact details (if you would like to be credited)

## Response Expectations

When you report a vulnerability, you can expect the following from the maintainers:

- **Acknowledgement within 48 hours** of receiving your report.
- **A triage update within 7 days** confirming whether the issue is accepted, needs more information, or is out of scope.
- **Regular updates** while a fix is being developed.
- **Coordinated disclosure:** we will agree on a disclosure timeline with you before any public advisory is published. Reporters who wish to be credited will be acknowledged in the GitHub Security Advisory.

## Scope

In scope:

- Bash scripts and installation logic in this repository (`sdkman/sdkman-cli`)

Out of scope for this policy — please report to the appropriate destination:

- **Native CLI commands** — report via [sdkman-cli-native](https://github.com/sdkman/sdkman-cli-native)
- **The SDKMAN! API and backend services** (e.g. `api.sdkman.io`, candidate distribution) — report privately to [security@sdkman.io](mailto:security@sdkman.io)
- **Candidate binaries** (JDKs, Maven, Gradle, etc.) — these are published by their respective vendors; please report to them directly
- **Issues in third-party dependencies** unless SDKMAN! CLI's use of them is itself the vulnerability
- Denial-of-service, brute-force, social engineering, or physical attacks against any sdkman.io infrastructure

## Questions

If you are unsure whether an issue qualifies as a security vulnerability, err on the side of caution and report it privately using one of the channels above.
