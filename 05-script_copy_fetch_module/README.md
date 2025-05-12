# Execute Script on Remote Hosts

This playbook demonstrates how to:

- Copy a script (`sc.sh`) to remote hosts using the `copy` module
- Fetch the script back to the local machine using the `fetch` module
- Execute the script on remote hosts using the `script` module
- Display the output of the script

## How to Run

For run The Script:
```bash
ansible-playbook -i inventory/hosts.yml project.yml --tags "script_sc"
```

Copy the File
```bash 
ansible-playbook -i inventory/hosts.yml project.yml --tags "copy_sc"
```

Fetch the File
```bash
ansible-playbook -i inventory/hosts.yml project.yml --tags "fetch_sc"
```


