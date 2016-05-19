# selenium-grid-ansible

This script uses Ansible 2 specific syntax. To install Ansible 2 on Ubuntu:

```
$ sudo apt-get install software-properties-common
$ sudo apt-add-repository ppa:ansible/ansible
$ sudo apt-get update
$ sudo apt-get install ansible
```

For other systems (Raspberry Pi, Debian...) use Pip:

```
$ pip install ansible
```

Before running the script setup a machine or two with non-root sudo users selenium. Then edit the hosts files to include the ip addresses of the machines and do

```
$ ansible-playbook playbook.yml -i hosts -u selenium
```
