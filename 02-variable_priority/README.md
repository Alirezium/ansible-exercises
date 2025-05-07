# Ansible Variable Precedence Demo

This project demonstrates the precedence of variables in Ansible using a structured role setup.


## Variable Precedence (Highest to Lowest)

See `priority.txt` for notes. Ansible will apply variables based on the following precedence:

1. Extra vars (via command line)
2. Inline vars in `tasks/main.yml`
3. `vars/main.yml`
4. `vars/vars2.yml`
5. `vars/vars1.yml`
6. Default values (if used)

## How to Run

```bash
ansible-playbook -i inventory/hosts.yml project.yml
```

to test with extra vars:
```bash
ansible-playbook -i inventory/hosts.yml project.yml -e "myvar=value"
```
