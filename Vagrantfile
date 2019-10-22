# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  # Karuta port
  config.vm.network :forwarded_port, guest: 8080, host: 8080
  # Frontail port
  config.vm.network :forwarded_port, guest: 9001, host: 9001
  config.vm.provision :shell, path: "bootstrap.sh"
  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "karuta.yml"
  end
end
