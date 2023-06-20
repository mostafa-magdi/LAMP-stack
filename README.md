# LAMP-stack
# which is LAMP stack is a popular open-source solution stack used primarily in web development. LAMP consists of four components necessary to establish a fully functional web development environment: Linux, Apache, MySQL, and PHP. Together, they provide a proven set of software for delivering high-performance web applications

# before we start what is Ansible?
Ansible is an open source automation and orchestration tool for software provisioning, configuration management, and software deployment 
here we use ansible to perform LAMP-STACK

## Prerequisites
Ansible (installed on the control node)
SSH (installed on both the control node and remote machine/s)
Sudoer account with passwordless sudo (setup on remote machine/s, ensure that the remote user for all machines are the same or modify the inventory file to specify the respective remote user for each)

# Tested On
- Centos 9

# Directory Structure
```
project/
├── index.php
├── inventories
│   └── hosts
├── lamp-playbook.yml
└── roles
    └── lampstack
        ├── defaults
        │   └── main.yml
        ├── handlers
        │   └── main.yml
        ├── tasks
        │   └── main.yml
        ├── templates
        │   └── index.php.j2
        └── vars
```
