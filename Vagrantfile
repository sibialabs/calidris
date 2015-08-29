# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
  config.vm.box = "cent7-ruby"
  config.vm.box_url = "https://s3-us-west-2.amazonaws.com/shrike/cent7-ruby.box"

  config.vm.network "forwarded_port", guest: 3000, host: 3000
  config.vm.network "forwarded_port", guest: 6379, host: 6379
  config.vm.network "forwarded_port", guest: 9200, host: 9200

  config.vm.provider "virtualbox" do |vb|
    vb.cpus   = "2"
    vb.memory = "4096"
  end

end
