# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|

  config.vm.box = "bento/ubuntu-20.04"
  config.vm.hostname = "koldchain"
  config.vm.boot_timeout = 300



  # # config.vm.network "forwarded_port", guest: 3000, host: 3000
  # config.vm.network "forwarded_port", guest: 8000, host: 8000
  # config.vm.network "forwarded_port", guest: 5432, host: 1234 
  # config.vm.network "forwarded_port", guest: 52930, host: 52930 

  config.vm.network "private_network", ip: "192.168.56.1"



  config.vm.synced_folder "./", "/home/vagrant/koldchain"


  config.vm.provider "virtualbox" do |vb|

    vb.gui = false

    vb.memory = "3084"
  end

  config.vm.provision "shell", inline: <<-SHELL

  SHELL
end
