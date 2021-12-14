Jenkins Vagrant Ansible
=======================

A Vagrantfile and Ansible playbook to quickly fire up a Jenkins install.


Overview
--------

The Vagrantfile uses bento/ubuntu and creates a private network, giving the host the address 192.168.56.0.

The Ansible playbook  installs Jenkins



Usage
-----

```bash
$ git clone https://github.com/abzilla786/ansible-jenkins
$ cd jenkins-vagrant-ansible
$ vagrant up
```

Then visit http://192.168.56.0:8080 to complete the installation.