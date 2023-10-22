
Vagrant.configure("2") do |config|
  config.vm.provider "virtualbox" do |vb|
    vb.name = "zabbix-server"
    vb.memory = 2048
    vb.cpus = 2
  end
  config.vm.box = "ubuntu/focal64"
  config.vm.network "public_network", ip: "192.168.0.180"
  config.vm.provision "shell", path: "zabbix.sh"
end