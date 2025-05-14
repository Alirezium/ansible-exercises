# Shell Module Exercise

This playbook demonstrates how to use the `shell` module in Ansible.

## Tasks performed:
1. Run the `uptime` command on remote hosts.
2. Print the output.
3. Save the output into a log file at `/var/log/uptime.log` on each host.

## How to Run

```bash
ansible-playbook -i inventory/hosts.yml project.yml
```
