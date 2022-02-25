<!--
SPDX-FileCopyrightText: 2020 Helmholtz Centre for Environmental Research (UFZ)
SPDX-FileCopyrightText: 2020 Helmholtz-Zentrum Dresden-Rossendorf (HZDR)

SPDX-License-Identifier: Apache-2.0
-->

# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

Group your changes into these categories:

`Added`, `Changed`, `Deprecated`, `Removed`, `Fixed`, `Security`.

## Unreleased

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v1.1.1...main)

### Fixed

- Fix failing CI pipeline
  ([!57](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/57)
  by [tobiashuste](https://gitlab.com/tobiashuste)).

### Changed

- Install Keepalived 2.2.7 by default
  ([!58](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/58)
  by [christian.hueser.hzdr](https://gitlab.com/christian.hueser.hzdr)).

## [1.1.1](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v1.1.1) - 2021-07-08

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v1.1.0...v1.1.1)

### Fixed

- Fix failing built of Keepalived from source with module make in initial dry-runs
  ([!55](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/55)
  by [christian.hueser.hzdr](https://gitlab.com/christian.hueser.hzdr)).

## [1.1.0](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v1.1.0) - 2021-06-28

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v1.0.0...v1.1.0)

### Added

- Automate Ansible Galaxy role import
  ([!50](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/50)
  by [Normo](https://gitlab.com/Normo)).

### Changed

- Bump keepalived from 2.2.1 to 2.2.2
  ([!53](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/53)
  by [Normo](https://gitlab.com/Normo)).
- Use FQDN for Ansible modules
  ([!52](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/52)
  by [Normo](https://gitlab.com/Normo)).
- Make a dry-run part of molecule default scenario
  ([!49](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/49)
  by [Normo](https://gitlab.com/Normo)).

## [1.0.0](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v1.0.0) - 2021-01-26

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v0.5.0...v1.0.0)

### Added

- Add keepalived config verification task
  ([!42](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/42)
  by [Normo](https://gitlab.com/Normo)).

### Changed

- Resolve "Refactor file path variables"
  ([!35](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/35)
  by [Normo](https://gitlab.com/Normo)).
- Set keepalived 2.2.1 as default version
  ([!37](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/37)
  by [Normo](https://gitlab.com/Normo)).
- Remove keepalived user and group
  ([!39](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/39)
  by [Normo](https://gitlab.com/Normo)).
- Update role meta information
  ([!38](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/38)
  by [Normo](https://gitlab.com/Normo)).
- Rename default branch to 'main'
  ([!41](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/41)
  by [Normo](https://gitlab.com/Normo)).
- Update virtual env packages
  ([!43](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/43)
  by [Normo](https://gitlab.com/Normo)).
- Add variable to configure `max_auto_priority`
  ([!44](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/44)
  by [Normo](https://gitlab.com/Normo)).

## [0.5.0](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v0.5.0) - 2021-01-21

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v0.4.0...v0.5.0)

### Upgrade notes

The keepalived executable has been moved from the build directory
`/usr/local/src/keepalived-x.y.z/sbin/keepalived` to
`/usr/local/sbin/keepalived`. Due to this fact, the build directory of the
previous version is not removed during an upgrade. This needs to be done
manually.

### Changed

- Put sysconfig file into config directory
  ([!12](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/12)
  by [christian.hueser.hzdr](https://gitlab.com/christian.hueser.hzdr))
- Simplify systemd config reload
  ([!30](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/30)
  by [Normo](https://gitlab.com/Normo)).
- Use a temporary directory as build directory
  ([!34](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/34)
  by [Normo](https://gitlab.com/Normo)).

### Fixed

- Resolve "Upgrading Keepalived executable does not work as expected due to
  wrong path variables"
  ([!32](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/32)
  by [christian.hueser.hzdr](https://gitlab.com/christian.hueser.hzdr)).

## [0.4.0](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v0.4.0) - 2020-11-11

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v0.3.0...v0.4.0)

### Added

- Enable check-mode
  ([!27](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/27)
  by [Normo](https://gitlab.com/Normo)).

## [0.3.0](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v0.3.0) - 2020-09-25

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v0.2.1...v0.3.0)

### Changed

- Enable keepalived process tracking
  ([!19](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/19)
  by [tobiashuste](https://gitlab.com/tobiashuste)).
- Make CI jobs interruptible to support auto-cancellation
  ([!21](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/21)
  by [tobiashuste](https://gitlab.com/tobiashuste)).
- Cache pipenv dependencies in .gitlab-ci.yml
  ([!22](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/22)
  by [tobiashuste](https://gitlab.com/tobiashuste))

### Fixed

- Fix runtime directory not being available after reboot
  ([!20](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/20)
  by [tobiashuste](https://gitlab.com/tobiashuste)).

## [0.2.1](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v0.2.1) - 2020-08-20

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v0.2.0...v0.2.1)

### Fixed

- Fix mandatory variables check for `keepalived_virtual_ipaddress_configs`
  ([!17](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/17)
  by [tobiashuste](https://gitlab.com/tobiashuste)).

## [0.2.0](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v0.2.0) - 2020-08-18

[List of commits](https://gitlab.com/hifis/ansible/keepalived-role/-/compare/v0.1.0...v0.2.0)

### Added

- Optionally allow to specify multiple virtual IP addresses
([!16](https://gitlab.com/hifis/ansible/keepalived-role/-/merge_requests/16)
by [tobiashuste](https://gitlab.com/tobiashuste)).

## [0.1.0](https://gitlab.com/hifis/ansible/keepalived-role/-/releases/v0.1.0) - 2020-08-14

### Added

Initial release of the Ansible Keepalived Role.
