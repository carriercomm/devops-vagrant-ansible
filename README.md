DevOps - Vagrant / Ansible project structure
=============================================

References
-------------

- [Ansible Provisioning - Vagrant Documentation](https://docs.vagrantup.com/v2/provisioning/ansible.html)
- [Ansible Galaxy — Ansible Documentation](http://docs.ansible.com/galaxy.html)
- [ansible/ansible-examples](https://github.com/ansible/ansible-examples)
- [geerlingguy/ansible-vagrant-examples](https://github.com/geerlingguy/ansible-vagrant-examples)
    - [geerlingguy/ansible-for-devops](https://github.com/geerlingguy/ansible-for-devops)
- [bcoe/librarian-ansible](https://github.com/bcoe/librarian-ansible)
- [Leonid Mirsky - Creating hadoop test environment with ansible and vagrant](http://leonidmirsky.com/ansible/hadoop/devops/2013/11/19/creating-hadoop-test-environment-with-ansible-and-vagrant.html)

Snippets
----------------
    
    echo "127.0.0.1" > ~/.ansible_hosts
    export ANSIBLE_HOSTS=~/.ansible_hosts

    ansible-galaxy install -r ansible/requirements.yml -p ansible/roles/ --force --ignore-errors
