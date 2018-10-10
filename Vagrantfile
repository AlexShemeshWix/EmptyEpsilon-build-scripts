# -*- mode: ruby -*-
# vi: set ft=ruby :

## Rename this to Vagrantfile to have 'vagrant up' work properly

###32bit Debian 9 Vagrant VM
### for EmptyEpsilon https://github.com/daid/EmptyEpsilon
### By Kwadroke "of The Wired" https://github.com/kwadroke

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/bionic64"
  config.ssh.forward_x11 = true
  config.vm.provider "virtualbox" do |vb|
    vb.cpus = 4
    vb.memory = 4096
  config.vm.provision :shell, path: "build_ee_u1804.sh", run: 'always'
   
  end

  config.vm.hostname = "bridgesim-ee"


end
