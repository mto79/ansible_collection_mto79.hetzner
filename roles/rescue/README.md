# [Checkmk-Server](#checkmk-server)

CheckMK role to install server

## [Requirements](#requirements)

* The minimum version of Ansible required is 2.10.
* The minimum version of Jinja template 2.11.3

## [Example Playbook](#example-playbook)

```yaml
---
- name: playbook
  hosts: all
  become: yes
  gather_facts: yes

  roles:
    - { role: proxyservices.checkmk.server, tags: ['checkmk', 'server', 'application'] }

  collections:
    - proxyservices.checkmk.server

```

## [Role variables](#role-variables)

| Variable | Default | Description |
| -------- | ------- | ----------- |
| `checkmk_server_opsgenie_enable` | `false` | Enable/Disable opsgenie integration
| `checkmk_server_opsgenie_team` | `Empty` | Assign Opsgenie team
| `checkmk_server_opsgenie_heartbeat` | `Empty` |  Assign Opsgenie heartbeat

## [Standards](#standards)

* [KT1 - Code manifesto](https://proxymanagedservices.atlassian.net/wiki/spaces/KT1/pages/255197272/Code+Manifest)
* [MST - Standards](https://proxymanagedservices.atlassian.net/wiki/spaces/PROD/pages/258703444/Ansible+Standards)

## [Maintainers](#maintainers)

* @nbaay
* @mouwerkerk
* @bversluis
* @jvdberg
* @eprinsen
* @jvrolijk

## [Todo](#todo)

* Standaardwaarden voor molecule testen toevoegen

## [License](#license)

Proprietary, MST Proxy B.V.
