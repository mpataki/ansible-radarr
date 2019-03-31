# ansible-radarr

[![Build Status](https://travis-ci.org/mpataki/ansible-radarr.svg?branch=master)](https://travis-ci.org/mpataki/ansible-radarr)

This role installs, configures, and runs [radarr](https://radarr.video/).

## Requirements

This role was tested on a raspberry pi running raspbian (stretch).

## Role Variables

These variables are largely straight out of the radarr config file. See [config.xml](templates/config.xml) and the [defaults](defaults/main.yml).

## Dependencies

None.

## Example Playbook

```yml
    - hosts: pi
      roles:
        - role: mpataki.radarr
          tags: radarr
          vars:
            radarr_version: 0.2.0.1293
```
