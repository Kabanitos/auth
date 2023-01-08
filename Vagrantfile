# -*- mode: ruby -*-
# vim: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "file:///hdd/hdd1/packer/Centos/packer_centos7/centos7-minimal.box"
  config.ssh.insert_key = false

    config.vm.provider "virtualbox" do |vb|
      vb.name = "auth"
      vb.gui = false
      vb.memory = "2048"
      vb.cpus = 1
    end
  config.vm.hostname = "auth"
  config.vm.network "public_network"
    config.vm.provision "shell" do |s|
      ssh_pub_key = File.readlines("/home/alex/.vagrant.d/insecure_private_key").first.strip
          s.inline = <<-SHELL
          echo #{ssh_pub_key} >> /home/vagrant/.ssh/authorized_keys
          SHELL
      end
     
  end



