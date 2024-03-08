# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "debian/buster64"
config.vm.provider "virtualbox" do |vb|
    vb.name = "newapp"
    vb.memory = "4096"
    vb.cpus = 2
end
config.vm.hostname = "newapp"

  config.vm.synced_folder ".", "/home/vagrant/code",
    owner: "www-data", group: "www-data"
  
  config.vm.network "forwarded_port", guest: 80, host: 8000
  config.vm.network "forwarded_port", guest: 3306, host: 33060

  config.vm.network "public_network", ip: "192.168.50.11"

#  config.vm.provision "shell", path: "provision.sh"
end
