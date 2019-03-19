[![Build Status](https://www.travis-ci.org/securCom/ansible-role_repo-openvpn.svg?branch=master)](https://www.travis-ci.org/securCom/ansible-role_repo-openvpn)
[![GitHub release](https://img.shields.io/github/release/securCom/ansible-role_repo-openvpn.svg)](https://github.com/securCom/ansible-role_repo-openvpn)


# Repo: OPENVPN

Manage OPENVPN official repositories.

# Requirements

For supported systems  and instructions see https://community.openvpn.net/openvpn/wiki/OpenvpnSoftwareRepos. If your system is not supported, the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `openvpn_repo_version`: the openvpn version to install (__stable__, __testing__ or __release/2.3__)
- `openvpn_repo_state`: define presence of the repository

# Dependencies

There no external dependencies.

# Example Playbook

To install role, add following line to **ansible-galaxy** requirements file
```
- src: https://github.com/securCom/ansible-role_repo-openvpn
  version: master
  name: securcom.repo_openvpn
```

```
- hosts: servers
  roles:
     - securcom.repo_openvpn
```

# License

BSD

# Author Information


- Peter Hudec (@hudecof)