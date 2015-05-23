DevOps - Vagrant / Ansible project structure
=============================================

Requirements
---------------

- [VirtualBox](https://www.virtualbox.org/)
    - <https://www.virtualbox.org/wiki/Downloads>
- [Vagrant](http://www.vagrantup.com/)
    - <http://www.vagrantup.com/downloads.html>
- [Ansible](http://www.ansible.com/)
    - <http://docs.ansible.com/intro_installation.html>


Installation
----------------
    
    $ ansible-galaxy install -r ansible/requirements.yml -p ansible/roles/galaxy --force --ignore-errors
    $ vagrant up


Known Issues
---------------

- [`vagrant up` hangs at "Waiting for VM to boot. This can take a few minutes" · mitchellh/vagrant Wiki](https://github.com/mitchellh/vagrant/wiki/%60vagrant-up%60-hangs-at-%22Waiting-for-VM-to-boot.-This-can-take-a-few-minutes%22)


References
-------------

- [Ansible Provisioning - Vagrant Documentation](https://docs.vagrantup.com/v2/provisioning/ansible.html)
- [Ansible Galaxy — Ansible Documentation](http://docs.ansible.com/galaxy.html)
- [ansible/ansible-examples](https://github.com/ansible/ansible-examples)
- [geerlingguy/ansible-vagrant-examples](https://github.com/geerlingguy/ansible-vagrant-examples)
    - [geerlingguy/ansible-for-devops](https://github.com/geerlingguy/ansible-for-devops)
- [bcoe/librarian-ansible](https://github.com/bcoe/librarian-ansible)
- [Leonid Mirsky - Creating hadoop test environment with ansible and vagrant](http://leonidmirsky.com/ansible/hadoop/devops/2013/11/19/creating-hadoop-test-environment-with-ansible-and-vagrant.html)
- [An example of provisioning and deployment with Ansible - Stavros' Stuff](http://www.stavros.io/posts/example-provisioning-and-deployment-ansible/)



