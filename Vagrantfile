# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.define "dotfiles-test" do |test|
    test.vm.box = "bento/ubuntu-18.04"
    test.vm.provider "virtualbox" do |vb|
      vb.memory = "8192"
      vb.cpus = 4
      vb.name = "dotfiles-test"
    end
    test.vm.provision "shell", run: "always", inline: <<-SHELL
      sudo ip route del default
    SHELL
  end

  config.vm.define "dotfiles-dev" do |dev|
    dev.vm.box = "bento/ubuntu-24.04"
    dev.vm.provider "virtualbox" do |vb|
      vb.memory = "8192"
      vb.cpus = 4
      vb.name = "dotfiles-dev"
    end
  end
end
