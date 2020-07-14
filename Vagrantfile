# This guide is optimized for Vagrant 1.8 and above.
# Older versions of Vagrant put less info in the inventory they generate.
Vagrant.require_version ">= 1.8.0"


MEMORY=1024
DOMAIN="nozesnet"


Vagrant.configure(2) do |config|
  config.ssh.password = "vagrant"
  config.ssh.insert_key = true
  config.vm.provision "shell",
     run: "always",
     inline: "systemctl stop firewalld ; yum install lsof net-tools -y"

  config.vm.define "solr-1" do |v|
   v.vm.box = "solr-1"
   v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
   v.vm.host_name = "solr-1.#{DOMAIN}"
   v.vm.network "private_network", ip: "192.168.1.10" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
   v.vm.provider "virtualbox" do |virtualbox|
     virtualbox.name = "solr-1"
     virtualbox.memory = MEMORY
     virtualbox.cpus = 1
 end
end
config.vm.define "solr-2" do |v|
 v.vm.box = "solr-2"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "solr-2.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.11" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "solr-2"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
end
end
config.vm.define "solr-3" do |v|
 v.vm.box = "solr-3"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "solr-3.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.12" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "solr-3"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
end
end
config.vm.define "solr-4" do |v|
 v.vm.box = "solr-4"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "solr-4.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.13" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "solr-4"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
end
end
 config.vm.define "hbase-1" do |v|
  v.vm.box = "hbase-1"
  v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
  v.vm.host_name = "hbase-1.#{DOMAIN}"
  v.vm.network "private_network", ip: "192.168.1.20" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
  v.vm.provider "virtualbox" do |virtualbox|
    virtualbox.name = "hbase-1"
    virtualbox.memory = MEMORY
    virtualbox.cpus = 1
 end
end

 config.vm.define "hbase-2" do |v|
  v.vm.box = "hbase-2"
  v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
  v.vm.host_name = "hbase-2.#{DOMAIN}"
  v.vm.network "private_network", ip: "192.168.1.21" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
  v.vm.provider "virtualbox" do |virtualbox|
    virtualbox.name = "hbase-2"
    virtualbox.memory = MEMORY
    virtualbox.cpus = 1
 end
end
config.vm.define "hbase-3" do |v|
 v.vm.box = "hbase-3"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "hbase-3.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.22" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "hbase-3"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
end
end
config.vm.define "hbase-4" do |v|
 v.vm.box = "hbase-4"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "hbase-4.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.23" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "hbase-4"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
end
end
 config.vm.define "mongo-1" do |v|
  v.vm.box = "mongo-1"
  v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
  v.vm.host_name = "mongo-1.#{DOMAIN}"
  v.vm.network "private_network", ip: "192.168.1.30" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
  v.vm.provider "virtualbox" do |virtualbox|
    virtualbox.name = "mongo-1"
    virtualbox.memory = MEMORY
    virtualbox.cpus = 1
  end
 end

 config.vm.define "mongo-2" do |v|
  v.vm.box = "mongo-2"
  v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
  v.vm.host_name = "mongo-2.#{DOMAIN}"
  v.vm.network "private_network", ip: "192.168.1.31" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
  v.vm.provider "virtualbox" do |virtualbox|
    virtualbox.name = "mongo-2"
    virtualbox.memory = MEMORY
    virtualbox.cpus = 1
  end
 end
 config.vm.define "mongo-3" do |v|
  v.vm.box = "mongo-3"
  v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
  v.vm.host_name = "mongo-3.#{DOMAIN}"
  v.vm.network "private_network", ip: "192.168.1.32" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
  v.vm.provider "virtualbox" do |virtualbox|
    virtualbox.name = "mongo-3"
    virtualbox.memory = MEMORY
    virtualbox.cpus = 1
  end
 end

 config.vm.define "mongo-4" do |v|
  v.vm.box = "mongo-4"
  v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
  v.vm.host_name = "mongo-4.#{DOMAIN}"
  v.vm.network "private_network", ip: "192.168.1.33" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
  v.vm.provider "virtualbox" do |virtualbox|
    virtualbox.name = "mongo-4"
    virtualbox.memory = MEMORY
    virtualbox.cpus = 1
  end
 end

config.vm.define "es-1" do |v|
 v.vm.box = "es-1"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "es-1.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.40" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "es-1"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
 end
end
config.vm.define "es-2" do |v|
 v.vm.box = "es-2"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "es-2.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.41" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "es-2"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
 end
end

config.vm.define "es-3" do |v|
 v.vm.box = "es-3"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "es-3.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.42" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "es-3"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
 end
end

config.vm.define "es-4" do |v|
 v.vm.box = "es-4"
 v.vm.box_url = '/home/marcelo.cmotta/boxes/package.box'
 v.vm.host_name = "es-4.#{DOMAIN}"
 v.vm.network "private_network", ip: "192.168.1.43" #, gw: "192.168.0.1" , subnet: "255.255.255.0" #auto_config: "false"
 v.vm.provider "virtualbox" do |virtualbox|
   virtualbox.name = "es-4"
   virtualbox.memory = MEMORY
   virtualbox.cpus = 1
 end
end
config.vm.provision "ansible" do |ansible|
  ansible.verbose = "v"
  ansible.playbook = "/home/marcelo.cmotta/Desktop/Code/ansible/nosql.yml"
  #ansible.galaxy_roles_path = "/home/marcelo.cmotta/Desktop/Code/ansible/roles"
end
end
