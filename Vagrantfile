# -*- mode: ruby -*-
# vim: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "file:///hdd/hdd1/packer/Centos/packer_centos7/centos7.box"
  config.vm.network "public_network", bridge: "enp0s31f6"
  config.vm.hostname = "auth"
  config.vm.define "auth"
  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.memory = "2048"
    vb.name = "auth"
    vb.cpus = 1
  end
end



















#
#  config.ssh.insert_key = false
#
 #   config.vm.provider "virtualbox" do |vb|
  #    vb.name = "auth"
   #   vb.gui = false
    #  vb.memory = "2048"
     # vb.cpus = 1
      #vb.vm.network "public_network"
   #end
 #config.vm.hostname = "auth"  
 #end



