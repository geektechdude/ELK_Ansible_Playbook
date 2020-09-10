# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
   config.vm.box = "centos/7"
   
   config.ssh.insert_key = false
   
   config.vm.synced_folder ".","/vagrant", disabled: true

   config.vm.provider:virtualbox do |v|
    v.memory = 2048
    v.cpus = 1
    v.linked_clone = true
   end

   config.vm.define "elk1" do |elk|
    elk.vm.hostname = "elk1.test"
    elk.vm.network:private_network, ip:"192.168.28.71"
   end

   config.vm.define "elk2" do |elk|
    elk.vm.hostname = "elk2.test"
    elk.vm.network:private_network, ip:"192.168.28.72"
    elk.vm.network:forwarded_port, guest:5601, host: 5601
   end

   config.vm.define "elk3" do |elk|
    elk.vm.hostname = "elk3.test"
    elk.vm.network:private_network, ip:"192.168.28.73"
   end

   config.vm.define "elk4" do |elk|
    elk.vm.hostname = "elk4.test"
    elk.vm.network:private_network, ip:"192.168.28.74"
   end

   config.vm.define "elk5" do |elk|
    elk.vm.hostname = "elk5.test"
    elk.vm.network:private_network, ip:"192.168.28.75"
   end
 
end
