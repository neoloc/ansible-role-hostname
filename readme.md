Hostname Role
=========

This roles purpose is to configure the hostname, and store the FQDN and Shortname for other roles.

[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-neoloc.hostname-blue.svg)](https://galaxy.ansible.com/neoloc/ansible-role-hostname/)

Requirements
------------

All included in ansible-base package.

Role Variables
--------------

| Variable                | Required | Default | Choices                   | Comments                                 |
|-------------------------|----------|---------|---------------------------|------------------------------------------|
| hostname.fqdn           | yes      | N/A     | string value              | fully qualified domain name of host      |
| hostname.hostname       | yes      | N/A     | string value              | hostname (without domain part) of host   |

```yaml
hostname:
  fqdn: somehost.domain.tld
  hostname: somehost
```

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - neoloc.hostname

License
-------

See license.md

Author Information
------------------

[![Github](https://img.shields.io/badge/Github-neoloc-blue.svg)](https://github.com/neoloc)
