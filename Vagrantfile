# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.synced_folder '.', '/home/vagrant/synced', disabled: true
  config.vm.box = "maier/alpine-3.4-x86_64"

  config.vm.define :server do |host|
    _HOSTNAME = 'server'
    _PRIVATE_IP_ADDRESS = '192.168.33.10'

    host.vm.hostname = _HOSTNAME
    host.vm.network 'private_network', ip: _PRIVATE_IP_ADDRESS
  end
end
