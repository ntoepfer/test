# -*- mode: ruby -*-
# vi: set ft=ruby :
#

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"

  config.vm.provision "shell", inline: <<-SHELL
    yum install -y ansible
    cd /vagrant
    ansible-playbook -vv pc_lite.yml
  SHELL
end
