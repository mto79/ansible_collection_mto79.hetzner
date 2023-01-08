# [MTO79 - Ansible Collection - Hetzner](#mto79---ansible-collection---hetzner)

## [Description](#description)

Ansible collection that provisions Hetzner products like dedicated server or cloud instances.

## [Included content](#included-content)

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
[mto79.hetzner.cloud](https://github.com/mto79/ansible_collection_mto79.hetzner/blob/main/roles/cloud/README.md)| Provision Hetzner cloud with Ansible.| Tests currently unavailable.
<!--end collection content-->

## [Installing this collection](#installing-this-collection)

### Local

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

You can install the Hetzner collection with the Ansible Galaxy CLI:

    ansible-galaxy collection install mto79.hetzner

You can also include it in a `requirements.yml` file and install it with
`ansible-galaxy collection install -r requirements.yml`, using the format:

```yaml
---
collections:
  - name: mto79.hetzner
    version: X.Y.Z
```
## [Pre-commit](#pre-commit)

Install pre-commit

```bash
pip install pre-commit
```

Set hooks in .pre-commit-config.yaml

```bash
repos:
- repo: https://github.com/ansible/ansible-lint.git
  rev: v4.2.0
  hooks:
    - id: ansible-lint
      files: \.(yaml|yml)$
```

Enable pre-commit for your git repository

```bash
$ pre-commit install
pre-commit installed at .git/hooks/pre-commit
```

Testing pre-commit

```bash
pre-commit run --all-files
Ansible-lint.............................................................Passed
```

or just type:

```bash
git commit
```
## [More information](#more-information)

* [MTO Website](https://mto.nu)

## [Licensing](#licensing)

See [LICENSE](LICENSE).
