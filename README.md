## tinyproxy

[![Build Status](https://travis-ci.org/Oefenweb/ansible-tinyproxy.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-tinyproxy) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-tinyproxy-blue.svg)](https://galaxy.ansible.com/Oefenweb/tinyproxy)

Set up [tinyproxy](https://tinyproxy.github.io/) in Debian-like systems.

#### Requirements

None

#### Variables

* `tinyproxy_install`: [default: `[]`]: Additional packages to install

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - tinyproxy
```

#### License

MIT

#### Author Information

Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-tinyproxy/issues)!
