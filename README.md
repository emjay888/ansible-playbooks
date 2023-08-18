# DO Community - Ansible Playbooks

A collection of minimalist Ansible playbooks for automating server setups, based on DigitalOcean's Community guides.

- [WordPress with LAMP on Ubuntu 18.04](https://github.com/do-community/ansible-playbooks/tree/master/wordpress-lamp_ubuntu1804)

_\*the Initial Server Setup should be your starting point for fresh servers._

## Playbook Structure

The playbooks contained in this repository were created for educational purposes, and should serve as a base for you to create your own playbooks and roles.

Although we opt to not use roles, our playbooks follow a distinctive structure to facilitate reuse while keeping them mostly self-contained and straightforward.

For instance, this is how the `lamp` playbook is structured:

```
lamp_ubuntu
├── files
│   ├── info.php.j2
│   └── nginx.conf.j2
├── vars
│   └── default.yml
├── playbook.yml
└── readme.md
```
- `files/`: directory containing templates and other files required by the playbook.
- `vars/`: directory to save variable files. A `default.yml` var file is included by default.
- `playbook.yml`: the playbook file.
- `readme.md`: instructions and links related to this playbook.
