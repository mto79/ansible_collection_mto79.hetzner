# MTO79 - Ansible Collection - Hetzner

## Description
Ansible collection that provisions Hetzner products like dedicated server or cloud instances.

## Included content

<!--start collection content-->
### Lookup plugins
Name | Description
--- | ---

### Modules
Name | Description | Tests
--- | --- | ---

### Roles
Name | Description | Tests
--- | --- | ---
[mto79.hetzner.rescue](https://github.com/mto79/ansible_collection_mto79.hetzner/blob/main/roles/rescue/README.md)| Provision Hetzner dedicated server with rescue.| Tests currently unavailable.
<!--end collection content-->

## Installing this collection

### Locally

You can install the MTO79 Hetzner collection locally, if you acquired a tarball from the [releases page](https://github.com/mto79/ansible_collection_mto79.hetzner/releases) as follows:

    ansible-galaxy collection install /path/to/mto79-hetzner-X.Y.Z.tar.gz

You can also include it in a `requirements.yml` file and install it with
`ansible-galaxy collection install -r requirements.yml`, using the format:
```yaml
---
collections:
  - source: /path/to/mto79-hetzner-X.Y.Z.tar.gz
    type: file
```

### From the Galaxy

You can install the Checkmk collection with the Ansible Galaxy CLI:

    ansible-galaxy collection install mto79.hetzner

You can also include it in a `requirements.yml` file and install it with
`ansible-galaxy collection install -r requirements.yml`, using the format:

```yaml
---
collections:
  - name: mto79.hetzner
    version: X.Y.Z
```
## Licensing
See [LICENSE](LICENSE).