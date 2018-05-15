## tinyproxy

[![Build Status](https://travis-ci.org/Oefenweb/ansible-tinyproxy.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-tinyproxy) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-tinyproxy-blue.svg)](https://galaxy.ansible.com/Oefenweb/tinyproxy)

Set up [tinyproxy](https://tinyproxy.github.io/) in Debian-like systems.

#### Requirements

None

#### Variables

* `tinyproxy_install`: [default: `[]`]: Additional packages to install

* `tinyproxy_tinyproxy_conf`: [see: `defaults/main.yml`]: List of lines to be added to `/etc/tinyproxy.conf`

* `tinyproxy_port`: [default: `8888`]: The port which tinyproxy will listen on
* `tinyproxy_allow`: [default: `["{{ ansible_lo['ipv4']['address'] }}"]`]: Customization of authorization controls. If there are any access controls then the default action is to `DENY`. Otherwise, the default action is `ALLOW`. The order of the controls are important
* `tinyproxy_connect_port`: [default: `[443, 563]`]: This is a list of ports allowed when the `CONNECT` method is used. To disable the `CONNECT` method altogether, set the value to `0`.  If no item is found, all ports are allowed

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
