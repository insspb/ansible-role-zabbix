# Ansible Role: Zabbix

- Master branch: [![Build Status](https://travis-ci.org/insspb/ansible-role-zabbix.svg?branch=master)](https://travis-ci.org/insspb/ansible-role-zabbix)
- Developer branch: [![Build Status](https://travis-ci.org/insspb/ansible-role-zabbix.svg?branch=develop)](https://travis-ci.org/insspb/ansible-role-zabbix)

## Description
This role will install and configure zabbix monitoring agent, server and proxy on target host.
We use full templates for all zabbix config options, so you can configure you host in host_vars.
We do not install any database engine on server ourself (just package system install dependencies) so it is better to use another role to database configuration BEFORE zabbix install.

## Requirements
No requiments yet.

## Role Variables

## Supported OS matrix:

| OS | Zabbix Agent | Zabbix proxy | Zabbix server |
|:--|:-:|:-:|:-:|
| Ubuntu 14.04 x32 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| Ubuntu 14.04 x64 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| Ubuntu 16.04 x32 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| Ubuntu 16.04 x64 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| Debian 8 x32 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| Debian 8 x64 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| CentOS 6 x32 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| CentOS 6 x64 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| CentOS 7 | X (2.0.0) | X (2.0.0) | X (2.0.0) |
| Windows 8.1+ | X (No TLS) | | |

Last manually tested version in brackets.

## Dependencies
Independent role.

## Example Playbook

```yaml
- hosts: all
  gather_facts: true
  roles:
    - insspb.zabbix
```
## Development information

This role is developed with community help. 
Process of development follows this rule: 

 - You are free to add any pool request to develop branch. All request will be answered in timely manner. 
 - If you want to made any contribution, but do not know where to start - check issues.
 - Master branch updated just after significant changes in develop.
 - Please include documentation for new features. 
 - Please use variables.
 - Please do not forget to set defaults.
 - Please do your best to keep backward compatibility if possible.
 - Please use packet installation as default software installation method. Source installation must be optional anywhere if possible.
 - Please use official software developers repositories instead of general Debian/Ubuntu/Centos etc. 
 - Do you best to keep role independent from any other roles. User must have the way to choose what roles to use.

## License
MIT

## Author Information

This role is contributed and maintained by [Andrey Shpak](http://www.ashpak.ru). I am always available for [hire](https://www.upwork.com/o/profiles/users/_~01a780866aa29e4429/).
