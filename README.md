# ansible-role-sonarr

[![Build Status](https://travis-ci.org/dropsignal/ansible-role-sonarr.svg?branch=master)](https://travis-ci.org/dropsignal/ansible-role-sonarr)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-sonarr-blue.svg?style=flat)](https://galaxy.ansible.com/dropsignal/sonarr)
[![License](https://img.shields.io/badge/license-GPLv2-brightgreen.svg?style=flat)](COPYING)

Debian/RedHat - PVR for Usenet and BitTorrent users
Based off https://github.com/jewflix/ansible-role-jackett

## Requirements

None

## Role Variables

    sonarr_gid: 2000 (optional)
    sonarr_group: sonarr
    sonarr_uid: 2000 (optional)
    sonarr_owner: sonarr
    sonarr_home: /var/lib/sonarr
    sonarr_shell: /bin/bash
    sonarr_serverconfig:
      port: 8989
      adminpassword: ''
    sonarr_cpuquota: 100%

## Dependencies

None

## Example Playbook

    - hosts: mediaservers
      ansible.builtin.roles:
        - role: dropsignal.sonarr
          sonarr_home: /var/lib/sonarr
          sonarr_group: sonarr
          sonarr_owner: sonarr

## License

Copyright (C) 2021 Drop Signal

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License, version 2 as published by
the Free Software Foundation.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
