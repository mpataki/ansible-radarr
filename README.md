# ansible-radarr

This role installs, configures, and runs [radarr](https://radarr.video/).

## Requirements

Really this should work on any debian based system, but has been tested on a Raspberry Pi running Rasbian (stretch).

## Role Variables

These variables are largely straight out of the radarr config file. See [config.xm](templates/config.xml) and the [defaults](defaults/main.yml).

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
