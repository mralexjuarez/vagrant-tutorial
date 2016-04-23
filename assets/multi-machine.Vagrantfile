# Example Vagrantfile for multiple machines
# This file configures two machines with the hostnames of server and client.

Vagrant.configure(2) do |config|
  config.vm.define "server" do |server|
    server.vm.box = "centos6"
    server.vm.hostname = "server"
    server.vm.network "private_network", ip: "192.168.33.100"
    server.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.memory = "1024"
    end
  end
  config.vm.define "client" do |client|
    client.vm.box = "centos6"
    client.vm.hostname = "client"
    client.vm.network "private_network", ip: "192.168.33.200"
    client.vm.provider "virtualbox" do |vb|
      vb.gui = false
      vb.memory = "1024"
    end
  end
end
