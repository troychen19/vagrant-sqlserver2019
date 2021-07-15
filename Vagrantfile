
Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu-20.04"

  
  config.vm.box_check_update = false
  config.vbguest.auto_update = false

  config.vm.network "forwarded_port", guest: 1433, host: 1433

  config.vm.provider "virtualbox" do |vb|
     vb.gui = false
     vb.memory = "4096"
     vb.cpus = 4
  end
  
  config.vm.provision "shell", path: "install.sh"
end
