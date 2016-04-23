# This is an example Vagrantfile for a single machine

Vagrant.configure(2) do |config|
  config.vm.box = "centos7"
  config.vm.hostname = "server"
  config.vm.network "private_network", ip: "192.168.33.10"
   config.vm.provider "virtualbox" do |vb|
     vb.gui = true

     vb.memory = "1024"
   end
end
