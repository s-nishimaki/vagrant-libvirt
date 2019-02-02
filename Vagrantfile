# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define :node1 do |node|
    node.vm.box = "generic/ubuntu1604"
    node.vm.hostname = "libvirt-vm"
    node.vm.network "public_network", :dev => "enp2s0", :mode => 'bridge'

    node.vm.provider :libvirt do |v|
      v.cpus = 2
      v.memory = 2048
    end
  end
end
