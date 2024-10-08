# Changelog

All notable changes to this project will be documented in this file.
Each new release typically also includes the latest modulesync defaults.
These should not affect the functionality of the module.

## [v7.0.0](https://github.com/voxpupuli/puppet-augeasproviders_ssh/tree/v7.0.0) (2024-09-29)

[Full Changelog](https://github.com/voxpupuli/puppet-augeasproviders_ssh/compare/v6.0.0...v7.0.0)

**Breaking changes:**

- Drop support for multiple EOL OSes [\#110](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/110) ([traylenator](https://github.com/traylenator))

**Implemented enhancements:**

- Add support for Debian 12 and Fedora 40 [\#111](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/111) ([traylenator](https://github.com/traylenator))

**Closed issues:**

- cannot pull via the Forge [\#38](https://github.com/voxpupuli/puppet-augeasproviders_ssh/issues/38)

**Merged pull requests:**

- Drop redundant hiera files [\#109](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/109) ([traylenator](https://github.com/traylenator))
- Update git:// URLs to use https:// [\#94](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/94) ([herver](https://github.com/herver))
- Treat values as simple/array based on local lens [\#65](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/65) ([tedgarb](https://github.com/tedgarb))

## [v6.0.0](https://github.com/voxpupuli/puppet-augeasproviders_ssh/tree/v6.0.0) (2023-06-22)

[Full Changelog](https://github.com/voxpupuli/puppet-augeasproviders_ssh/compare/v5.0.0...v6.0.0)

**Breaking changes:**

- Drop Puppet 6 support [\#88](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/88) ([bastelfreak](https://github.com/bastelfreak))

**Implemented enhancements:**

- puppet/augeasproviders\_core: Allow 4.x [\#91](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/91) ([bastelfreak](https://github.com/bastelfreak))
- Add puppet 8 support [\#90](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/90) ([bastelfreak](https://github.com/bastelfreak))
- Add Rocky 9 support [\#87](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/87) ([bastelfreak](https://github.com/bastelfreak))
- Add support of PubkeyAcceptedKeyTypes for ssh\_config [\#81](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/81) ([hbenali](https://github.com/hbenali))

**Merged pull requests:**

- Fix incorrect Apache-2 license [\#85](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/85) ([bastelfreak](https://github.com/bastelfreak))
- Fix License detection [\#84](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/84) ([bastelfreak](https://github.com/bastelfreak))

## [v5.0.0](https://github.com/voxpupuli/puppet-augeasproviders_ssh/tree/v5.0.0) (2022-08-30)

[Full Changelog](https://github.com/voxpupuli/puppet-augeasproviders_ssh/compare/4.0.0...v5.0.0)

**Breaking changes:**

- Drop Non LTS Ubuntu 18.10/19.04/19.10; Add 22.04 [\#78](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/78) ([bastelfreak](https://github.com/bastelfreak))
- Drop Eol Debian 7/8/9; Add Debian 10/11 support [\#77](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/77) ([bastelfreak](https://github.com/bastelfreak))
- Drop RHEL 6 support [\#76](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/76) ([bastelfreak](https://github.com/bastelfreak))

**Merged pull requests:**

- cleanup README.md [\#79](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/79) ([bastelfreak](https://github.com/bastelfreak))
- Move Forge org to "puppet" [\#73](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/73) ([op-ct](https://github.com/op-ct))
- Dependency and Support Bump [\#72](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/72) ([trevor-vaughan](https://github.com/trevor-vaughan))
- Fix HostKeyAlgorithms in sshd\_config [\#68](https://github.com/voxpupuli/puppet-augeasproviders_ssh/pull/68) ([loopiv](https://github.com/loopiv))

## [4.0.0](https://github.com/voxpupuli/puppet-augeasproviders_ssh/tree/4.0.0) (2020-07-16)

- Deprecate support for Augeas < 1.0.0
- Update supported Ubuntu versions
- sshd_config: close array regexp (GH #54), fix GH #52
- sshd_config_match: remove duplicated condition param in test (GH #58)
- sshkey: do not test type update, it's a parameter in Puppet 6 (GH #59)
- Add support for comments in types and providers (GH #61)
- Update copyright and authors infos

## 3.3.0

- Add EL8 support
- Add 'Port' to the list of items supporting Arrays in the documentation

## 3.2.1

- Fix puppet requirement to < 7.0.0

## 3.2.0

- add support for Puppet 5 & 6
- deprecate support for Puppet < 5
- update supported OSes in metadata.json

## 3.1.0

- Add support for array_append to sshd_config type (GH #43)

## 3.0.0

- Fix support for 'puppet generate types'
- Bumped supported puppet version to less than 6.0.0
- Updated the spec_helper.rb to correctly load for Puppet 5
- Added CentOS and OracleLinux to supported OS list

## 2.5.3

- ssh_config: fix HostKeyAlgorithms and KexAlgorithms (#GH 36)

## 2.5.2

- Added docker acceptance test
- Refactor the travis.yml for the current LTS versions of Puppet

## 2.5.1

- Bugfix Release:
  - Allow multiple values for GlobalKnownHostsFile (#GH 32)
  - Ensure that AddressFamily comes before ListenAddress (#GH 34)

## 2.5.0

- Implement instances for sshkey (only for non-hashed entries)

## 2.4.0

- Add sshd_config_match type and provider (#GH 5)
- Purge multiple array entries in ssh_config provider (GH #12)

## 2.3.0

- Add sshkey provider (GH #13)
- sshd_config: munge condition parameter
- Improve test setup
- Get rid of Gemfile.lock
- Improve README badges

## 2.2.2

- Properly insert values after commented out entry if case doesn't match (GH #6)

## 2.2.1

- Convert specs to rspec3 syntax
- Fix metadata.json

## 2.2.0

- sshd_config: consider KexAlgorithms and Ciphers as array values (GH #4)

## 2.1.0

- Add ssh_config type & provider

## 2.0.0

- First release of split module.


\* *This Changelog was automatically generated by [github_changelog_generator](https://github.com/github-changelog-generator/github-changelog-generator)*
