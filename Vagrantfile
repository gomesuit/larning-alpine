# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.synced_folder '.', '/vagrant', disabled: true
  config.vm.box = "maier/alpine-3.4-x86_64"
  config.ssh.forward_agent = true

  config.ssh.shell = '/bin/sh'
  config.vm.network :private_network, ip: '192.168.33.10', auto_config: false
end
