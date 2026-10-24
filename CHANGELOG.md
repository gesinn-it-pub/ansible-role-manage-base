# Changelog

All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](https://semver.org/) and
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

Releases before 2.0.0 are listed on the [GitHub releases page](https://github.com/gesinn-it-pub/ansible-role-manage-base/releases).

## [Unreleased]

## [2.0.0] - 2026-10-24

Raises the minimum ansible-core to 2.19 and removes a deprecated task file name. Make the changes under Breaking
Changes before you update.

### Breaking Changes
- Require ansible-core 2.19 or newer; 2.18 is no longer supported [`5335bee`](https://github.com/gesinn-it-pub/ansible-role-manage-base/commit/5335bee)
- Remove the task file `fix-python-EXTERNALLY_MANAGED.yml`; call `fix-python-externally-managed.yml` instead [`d976026`](https://github.com/gesinn-it-pub/ansible-role-manage-base/commit/d976026)

### Added
- Add `manage_base_docker_no_proxy` to set the `noProxy` list of the Docker client; the default is the previous fixed value [`3abd81f`](https://github.com/gesinn-it-pub/ansible-role-manage-base/commit/3abd81f)
- Add the task file `fix-python-externally-managed.yml` with the lowercase name [`1fc2b68`](https://github.com/gesinn-it-pub/ansible-role-manage-base/commit/1fc2b68)

### Changed
- Write `/root/.docker/config.json` as formatted JSON; the content stays the same, so the first run after the update reports the file as changed [`3abd81f`](https://github.com/gesinn-it-pub/ansible-role-manage-base/commit/3abd81f)
- Document usage, variables and handlers in the README [`c15ba7a`](https://github.com/gesinn-it-pub/ansible-role-manage-base/commit/c15ba7a)

[Unreleased]: https://github.com/gesinn-it-pub/ansible-role-manage-base/compare/2.0.0...HEAD
[2.0.0]: https://github.com/gesinn-it-pub/ansible-role-manage-base/compare/1.5.3...2.0.0
