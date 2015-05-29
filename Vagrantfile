#!/usr/bin/ruby
# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = '2'

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.box = 'ubuntu/trusty64'
    config.vm.box_version = '>= 14.04'

    # Default = 300
    config.vm.boot_timeout = 32000

    # Set to true for debugging
    config.vm.provider :virtualbox do |vb|
        vb.gui = false
    end

    # Automatically update VirtualBox Guest Additions
    # Requires vagrant-vbguest plugin
    # @see https://github.com/dotless-de/vagrant-vbguest
    config.vbguest.auto_update = true

    # LAMP Stack
    config.vm.define :lamp, primary: true do |lamp|
        lamp.vm.hostname = 'lamp'
        lamp.vm.network 'private_network', ip: '192.168.33.10'
        lamp.vm.provision :ansible do |ansible|
            ansible.playbook = 'ansible/playbook.yml'
            #ansible.inventory_path = 'ansible/inventories/FILENAME'
            ansible.limit = 'all'
            ansible.sudo = true
            ansible.verbose = true
        end
    end

end
