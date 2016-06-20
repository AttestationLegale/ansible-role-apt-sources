# Ansible Role: Apt sources

[![Build Status](https://travis-ci.org/AttestationLegale/ansible-role-apt-sources.svg?branch=master)](https://travis-ci.org/AttestationLegale/ansible-role-apt-sources) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-apt--sources-blue.svg)](https://galaxy.ansible.com/AttestationLegale/apt-sources/)

Manage apt `sources.list.d`.

## Requirements

None

## Role Variables

For a complete list of variables, see `default/main.yml`.

    apt_sources_entries: []
    apt_sources_group_entries: []
    apt_sources_host_entries: []

## Dependencies

None

## Example Playbook

```yaml
---
  - hosts: all
    roles:
      - apt-sources
    vars:
      apt_sources_entries:
        - url: "https://deb.nodesource.com/node_6.x"
          key: "https://deb.nodesource.com/gpgkey/nodesource.gpg.key"
```

## License

MIT / BSD

## Author Information

This role was created in 2016 by [ALG](https://www.attestationlegale.fr)
