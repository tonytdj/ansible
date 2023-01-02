# -*- mode: ruby -*-
# vi: set ft=ruby :

RAM = 2048
CPU = 2

Vagrant.configure("2") do |config|
  config.vm.define "ansible" do |ansible|
    ansible.vm.box = "generic/centos7"
    ansible.vm.network "private_network", type: "dhcp"
    ansible.vm.hostname = "ansible"
    #ansible.vm.synced_folder '.', '/vagrant', disabled: true
    ansible.vm.provider "virtualbox" do |v|
      v.name = "ansible"
      v.memory = RAM
      v.cpus = CPU
    end
  end
end