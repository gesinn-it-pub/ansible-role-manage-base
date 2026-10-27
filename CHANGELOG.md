# Changelog

All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](https://semver.org/) and
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Fixed
- Run the Docker network check on hosts whose `python3` is 3.6, e.g. Rocky Linux 8. It failed there with a Python error before anything else ran

### Changed
- Declare EL 8 (Rocky Linux) as a supported platform. The role has no distribution specific code; it is not covered by the Molecule scenarios, which do not run a real package manager or Docker daemon

## [3.0.0] - 2026-10-24

Stops installing the Traefik role. Make the change under Breaking Changes before you update.

### Breaking Changes
- Stop installing `gesinn.manage_traefik`; include it in your own play if you relied on this role for it, and keep it in your own `requirements.yml` [`d05aa1e`](https://github.com/gesinn-it-pub/ansible-role-manage-base/commit/d05aa1e)

[Unreleased]: https://github.com/gesinn-it-pub/ansible-role-manage-base/compare/3.0.0...HEAD
[3.0.0]: https://github.com/gesinn-it-pub/ansible-role-manage-base/compare/2.0.0...3.0.0

Older releases: [2.x](CHANGELOG-2.x.md)
