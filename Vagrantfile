Vagrant.configure("2") do |config|
 config.vm.box = "ubuntu/xenial64"

 config.vm.network "forwarded_port", guest: 80, host: 80
 config.vm.network "forwarded_port", guest: 8080, host: 8080
 config.vm.network "forwarded_port", guest: 8888, host: 8888
 config.vm.network "forwarded_port", guest: 3000, host: 3000
 config.vm.network "forwarded_port", guest: 5432, host: 5432

 config.vm.network "private_network", ip: "192.168.33.10"

 config.vm.provider "virtualbox" do |vb|
   vb.memory = "4096"
 end
end
