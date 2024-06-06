#  Ansible Playbook 

## Project Description:
In this project, I developed Ansible Playbook for Java, Apache, Tomcat and Nginx on Ubuntu. The primary goal of this project is to automated app installation and deployment.

## Overview:

## Prerequisites:

1. Basic knowledge of Linux and concepts.
2. Familiarity with Ansible command.
3. An IDE of your Choice , I would suggest VS Code Editor.

## Installation of Ansible on Ubuntu:
Ansible installation process on Ubuntu.

```
sudo apt-get update 
sudo apt-get install software-properties-common 
sudo apt-add-repository ppa:ansible/ansible 
sudo apt-get update 
sudo apt-get install ansible
```

## Quick Ad hoc Commands for Ansible:
Here is some Ansible Ad hoc Commands for quick use :

```
ansible all -m ping
ansible all -m setup
ansible all -m shell -a "uptime"
ansible all -m copy -a "src=/path/to/local/file dest=/path/to/remote/file"
ansible all -m file -a "path=/path/to/file state=touch"
ansible all -m service -a "name=httpd state=started"
ansible all -m apt -a "name=nginx state=present"
ansible all -m yum -a "name=httpd state=present"
ansible all -m user -a "name=username state=present"
ansible all -m file -a "path=/path/to/file owner=username group=groupname mode=0644"
ansible all -m command -a "ls /root" –b
ansible all -m command -a "df -h"
ansible all -m fetch -a "src=/path/to/remote/file dest=/path/to/local/dir"
ansible all -m synchronize -a "src=/path/to/local/dir dest=/path/to/remote/dir"
ansible all -m reboot
```

## Playbook :

### Playbook 1: Installation of Java using Ansible playbook with version

Install the Ansible and Run the Playbook

```
ansible-playbook -i inventory ansible_java_install.yml
```

### Playbook 2: Installation of Java using Ansible playbook with version

Install the Ansible and Run the Playbook

```
ansible-playbook -i inventory ansible_java_install_with_version_promt.yml
```

### Playbook 3: Installation of Apache using Ansible playbook

Install the Ansible and Run the Playbook

```
ansible-playbook -i inventory ansible_apache_install.yml
```

### Playbook 4: Installation of Tomcat using Ansible playbook with version

Install the Ansible and Run the Playbook

```
ansible-playbook -i inventory ansible_nginx_install.yml
```

### Playbook 5: Installation of Nginx using Ansible playbook

Install the Ansible and Run the Playbook

```
ansible-playbook -i inventory ansible_nginx_install.yml
```