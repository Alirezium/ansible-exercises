# Using Ansible Command Module to Show Disk Usage

This exercise demonstrates how to use Ansible's **command** module to run shell commands on remote hosts.  
Specifically, the `df -h` command is used to display disk usage in human-readable format.

## Playbook Tasks

The following tasks are defined in `roles/project/tasks/main.yml`:

```yaml
- name: -----show df -h-----
  command: df -h
  register: df
  tags: show_df

- name: -----show df-----
  debug:
    msg: "{{ df.stdout }}"
  tags: show_df
```

## How to Run

```bash
ansible-playbook -i inventory/hosts.yml project.yml --tags show_df
```
