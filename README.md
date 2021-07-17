# ansible-role-sonarr

[![Build Status](https://travis-ci.org/dropsignal/ansible-role-sonarr.svg?branch=master)](https://travis-ci.org/dropsignal/ansible-role-sonarr)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-sonarr-blue.svg?style=flat)](https://galaxy.ansible.com/dropsignal/sonarr)
[![License](https://img.shields.io/badge/license-GPLv2-brightgreen.svg?style=flat)](COPYING)

RedHat - Sonarr is a PVR for Usenet and BitTorrent users

## Requirements

None

## Role Variables

    sonarr_group: sonarr
    sonarr_home: /var/lib/sonarr
    sonarr_owner: sonarr
    sonarr_serverconfig:
      port: 8989
      adminpassword: ''

## Dependencies

None

## Example Playbook

    - hosts: mediaservers
      roles:
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
