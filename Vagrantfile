# This guide is optimized for Vagrant 1.8 and above.
# Older versions of Vagrant put less info in the inventory they generate.
Vagrant.require_version ">= 1.8.0"

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.provider "virtualbox" do |virtualbox|
      virtualbox.name = "ansible"
      virtualbox.memory = 1024
      virtualbox.cpus = 1

  
  config.vm.provision "ansible" do |ansible|
    ansible.verbose = "v"
    ansible.playbook = "playbook.yml"
 
 end
end
end
