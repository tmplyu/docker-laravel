# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "generic/ubuntu2004"

  config.vm.network "private_network", ip: "192.168.33.100"

  config.vm.synced_folder ".", "/home/vagrant/project"

  config.vm.provision "shell", path: "./provision/setup_root.sh"
end
