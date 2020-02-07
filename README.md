[![Build Status](https://travis-ci.org/bihealth/ansible-role-dnsmasq.svg?branch=master)](https://travis-ci.org/bihealth/ansible-role-dnsmasq)

# dnsmasq

Basic setup of dnsmasq.

Currently only sets up dnsmasq as a resolver.

## Requirements

None

## Role Variables

See `defaults/main.yml` for all role variables and their documentation.

## Dependencies

None

## Example Playbook

```yaml
- hosts: servers
  vars:
    dnsmasq_force_set_etc_resolv_conf: true
    dnsmasq_upstream_servers:
      - 8.8.8.8
      - 4.4.4.4
  roles:
    - role: bihealth.dnsmasq
```

## License

MIT

## Author Information

- Manuel Holtgrewe

Created with love at [Core Unit Bioinformatics (CUBI), Berlin Institute of Health (BIH)](https://www.cubi.bihealth.org).
