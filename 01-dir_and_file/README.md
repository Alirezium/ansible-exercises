# Ansible: Create Directories and Files

This Ansible playbook creates two directories and two files on the target system.

## What It Does

- Creates `/home/dir1` and `/home/dir1/file1`
- Creates `/home/dir2` and `/home/dir2/file2`

## Tags

You can run specific parts using tags:

- `dir1` – create `/home/dir1`
- `dir1/file1` – create `/home/dir1/file1`
- `dir2` – create `/home/dir2`
- `dir2/file2` – create `/home/dir2/file2`

## Usage

```bash
ansible-playbook playbook.yml
