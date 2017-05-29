# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "debian/jessie64"

  config.vm.define "vm1" do |vm1|
    vm1.vm.network "private_network", ip: "192.168.10.10"
    vm1.vm.network "private_network", ip: "10.10.20.10"
  end

  config.vm.define "vm2" do |vm2|
    vm2.vm.network "private_network", ip: "192.168.10.11"
    vm2.vm.network "private_network", ip: "10.10.30.10"
  end

  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
  
    vb.memory = "512"
  end
end
