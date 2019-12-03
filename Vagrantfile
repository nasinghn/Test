Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.hostname = "narender"
  
  config.vm.provision "shell", path: "provision.sh.txt"
  config.vm.network "forwarded_port", guest: 80, host: 8080, id: "nginx"
  #config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.synced_folder "html", "/vagrant/html"
  end