# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "chef/ubuntu-12.04"

  config.vm.network "forwarded_port", guest: 4000, host: 4000

  config.omnibus.chef_version = :latest
  config.berkshelf.enabled = true

  config.vm.provision :chef_solo do |chef|
    chef.add_recipe 'recipe[nodejs::default]'
    chef.add_recipe 'recipe[brightbox-ruby::default]'
  end

  config.vm.provision :shell, inline: 'cd /vagrant && bundle'
end
