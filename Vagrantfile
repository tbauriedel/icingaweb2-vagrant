# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-22.04"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/icingaweb2-single.yml"
  end
end
