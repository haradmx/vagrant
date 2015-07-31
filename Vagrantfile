# -*- mode: ruby -*-
# # vi: set ft=ruby :
#
# # Vagrantfile API/syntax version. Don't touch unless you know what you're doing!

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box_url = "https://github.com/haradmx/vagrant/releases/download/v0.1-alpha/iver-vagrant_v0.1-alpha.box"
  config.vm.box = "haradmx"
  config.vm.hostname = "harad"
  config.vm.network "private_network", ip: "10.2.2.204"
  config.vm.provision :shell, path: "bin/setup.sh"

  config.ssh.forward_agent = true

  config.vm.provider "virtualbox" do |vb|
    vb.customize ["modifyvm", :id, "--accelerate3d", "off"]
#    vb.customize [ "guestproperty", "set", :id, "/VirtualBox/GuestAdd/VBoxService/--timesync-set-threshold", 10000 ]
    vb.memory = 1024
    vb.cpus = 2
    vb.gui = true
  end
end
