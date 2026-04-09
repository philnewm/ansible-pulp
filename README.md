# Pulp-Role

[![Alma9-CI](https://github.com/philnewm/ansible-pulp/actions/workflows/alma9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-pulp/actions/workflows/alma9-ci-caller.yml)  [![Rocky9-CI](https://github.com/philnewm/ansible-pulp/actions/workflows/rocky9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-pulp/actions/workflows/rocky9-ci-caller.yml)  [![CentOSStream9-CI](https://github.com/philnewm/ansible-pulp/actions/workflows/centosstream9-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-pulp/actions/workflows/centosstream9-ci-caller.yml)  [![Debian13-CI](https://github.com/philnewm/ansible-pulp/actions/workflows/debian13-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-pulp/actions/workflows/debian13-ci-caller.yml)  [![Ubuntu2404-CI](https://github.com/philnewm/ansible-pulp/actions/workflows/ubuntu2404-ci-caller.yml/badge.svg)](https://github.com/philnewm/ansible-pulp/actions/workflows/ubuntu2404-ci-caller.yml)

Role description

This role includes a vagrant based molecule testing setup as a submodule at `molecule/`

## Structure

```code
📦 ansible-pulp
 ┣ 📂defaults
 ┃ ┗ 📂main
 ┃ ┃ ┣ 📜common.yml
 ┃ ┃ ┣ 📜python_repos.yml
 ┃ ┃ ┗ 📜rpm_repos.yml
 ┣ 📂meta
 ┃ ┗ 📜main.yml
 ┣ 📂 molecule
 ┃ ┗ 📂 default
 ┃   ┗ 📜, 📜, 📜, scenario_files
 ┣ 📂tasks
 ┃ ┣ 📜absent.yml
 ┃ ┣ 📜ansible_config.yml
 ┃ ┣ 📜container_config.yml
 ┃ ┣ 📜dependencies.yml
 ┃ ┣ 📜file_config.yml
 ┃ ┣ 📜main.yml
 ┃ ┣ 📜present.yml
 ┃ ┣ 📜pulp_cli.yml
 ┃ ┣ 📜python_config.yml
 ┃ ┣ 📜rpm_config.yml
 ┃ ┣ 📜service_setup.yml
 ┃ ┣ 📜tests.yml
 ┃ ┗ 📜verify_service.yml
 ┣ 📂vars
 ┃ ┗ 📜main.yml
 ┣ 📜.gitignore
 ┣ 📜.gitmodules
 ┣ 📜README.md
 ┗ 📜requirements.yml

```

Describe and explain role structure.

## Requirements

Elaborate external dependencies and how to use them.

## Role Variables

* defaults/main.yml
  * first_var
  * sec_var
  * third_var
* vars/main.yml
  * first_var
  * sec_var
  * third_var

## Dependencies

List role ansible-galaxy dependencies - if any.

## Example Playbook

Add an example playbook

```yaml
---

tasks:
  - name: Include ansible-pulp present
    ansible.builtin.include_role:
      name: ansible-pulp
    vars:
      state: present

...
```

## License

Add license - if any.
