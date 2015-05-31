DevOps - Vagrant / Ansible project structure
=============================================

Vagrant / Ansible Galaxy based LAMP stack and blank project structure


Requirements
---------------

- [VirtualBox](https://www.virtualbox.org/)
    - <https://www.virtualbox.org/wiki/Downloads>
- [Vagrant](http://www.vagrantup.com/)
    - <http://www.vagrantup.com/downloads.html>
    - [vagrant-vbguest plugin](https://github.com/dotless-de/vagrant-vbguest)
- [Ansible](http://www.ansible.com/)
    - <http://docs.ansible.com/intro_installation.html>


Installation
----------------
    
    $ ansible-galaxy install -r ansible/requirements.yml -p ansible/roles/vendor --force --ignore-errors
    $ vagrant up

### Hosts file

    192.168.33.10   project.dev


Known Issues
---------------

- [`vagrant up` hangs at "Waiting for VM to boot. This can take a few minutes" · mitchellh/vagrant Wiki](https://github.com/mitchellh/vagrant/wiki/%60vagrant-up%60-hangs-at-%22Waiting-for-VM-to-boot.-This-can-take-a-few-minutes%22)


References
-------------

### Docs

- [Ansible Provisioning - Vagrant Documentation](https://docs.vagrantup.com/v2/provisioning/ansible.html)
- [Playbook Roles and Include Statements — Ansible Documentation](http://docs.ansible.com/playbooks_roles.html)
- [Ansible Galaxy — Ansible Documentation](http://docs.ansible.com/galaxy.html)

### Code Examples

- [ansible/ansible-examples](https://github.com/ansible/ansible-examples)
- [geerlingguy/ansible-vagrant-examples](https://github.com/geerlingguy/ansible-vagrant-examples)
    - [geerlingguy/ansible-for-devops](https://github.com/geerlingguy/ansible-for-devops)
- [pesterhazy/vagrant-lamp-ansible](https://github.com/pesterhazy/vagrant-lamp-ansible/)
- [bcoe/librarian-ansible](https://github.com/bcoe/librarian-ansible)

### Articles

- [Leonid Mirsky - Creating hadoop test environment with ansible and vagrant](http://leonidmirsky.com/ansible/hadoop/devops/2013/11/19/creating-hadoop-test-environment-with-ansible-and-vagrant.html)
- [An example of provisioning and deployment with Ansible - Stavros' Stuff](http://www.stavros.io/posts/example-provisioning-and-deployment-ansible/)

### Troubleshooting

- [MySQL - Connect to your database remotely | Knowledge Center | Rackspace Hosting](https://www.rackspace.com/knowledge_center/article/mysql-connect-to-your-database-remotely)


Licence
---------

Unless explicitly noted otherwise, the content of this package is released under the [GNU Affero General Public License version 3 (AGPLv3)](http://www.gnu.org/licenses/agpl.html)

[Why the GNU Affero GPL](http://www.gnu.org/licenses/why-affero-gpl.html)

Copyright © 2014-2015 [Stéphane Thibault](http://www.cavalierblanc.com/).
