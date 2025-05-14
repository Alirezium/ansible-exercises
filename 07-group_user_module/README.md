# Ansible User and Group Creation

This exercise demonstrates how to use Ansible to:

- Create a group named `ansible`
- Create a user named `ansible`, assign it to the `ansible` group, set its shell to `/bin/bash`, and define its home directory

## How to Run

```bash
ansible-playbook -i inventory/hosts.yml project.yml
```
