# -*- mode: ruby -*-
# vi: set ft=ruby :

IP =  "192.168.58.93"   # Don't change!
CPU_CORES_COUNT = "8"   # Cnahge if necessary
MEMORY_COUNT = "16384"   # Cnahge if necessary

Vagrant.configure("2") do |osx|
    osx.vm.box = "jhcook/osx-elcapitan-10.11"
    osx.vm.synced_folder ".", "/vagrant", disabled: true
    osx.vm.network :private_network, ip: IP
    osx.vm.provider "virtualbox" do |vb|
        vb.name = "osx_elcapitan"
        vb.memory = MEMORY_COUNT
        vb.cpus = CPU_CORES_COUNT
        vb.gui = true
    end
  end