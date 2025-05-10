# Host-specific SSH Ports in Ansible

This exercise demonstrates how to use **host-specific variables** in the Ansible inventory to define different SSH ports for each host.

## Inventory

In the `inventory/hosts.yml` file, two hosts are defined with different SSH ports:

```ini
[myservers]
192.168.158.6 ansible_port=22
192.168.158.7 ansible_port=723
```

## How to Run

```bash
ansible-playbook -i inventory/hosts.yml project.yml --tags show_ssh_port
```
