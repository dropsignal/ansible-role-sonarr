# ansible-role-sonarr

Red Hat - Sonarr is a PVR for Usenet and BitTorrent users

## Requirements

None

## Role Variables

    jackett_cpuaccounting: false
    jackett_cpuquota: 100%
    jackett_group: jackett
    jackett_home: /opt/jackett
    jackett_owner: jackett
    jackett_serverconfig:
      Port: 9117
      AllowExternal: true
      APIKey: t0zpjpktkzx6ks5kiwk3diqp803phj7l
      AdminPassword: ''
      InstanceId: d8o15332wedlx8bnxdxd1m2ztoeo88wcf01z3uwlu5dm2t5wyxvjtj965vbs79t8
      BlackholeDir: ''
      UpdateDisabled: false
      UpdatePrerelease: false
      BasePathOverride: ''
      OmdbApiKey: ''
      OmdbApiUrl: ''
      ProxyUrl: ''
      ProxyType: 0
      ProxyPort: ''
      ProxyUsername: ''
      ProxyPassword: ''
      ProxyIsAnonymous: true
    jackett_shell: /sbin/nologin
    jackett_update: false

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
it under the terms of the GNU General Public License as published by
the Free Software Foundation, version 2 of the License.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
