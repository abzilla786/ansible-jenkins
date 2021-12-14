
Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-18.04"
  config.vm.box_check_update = "false"
  # config.vm.provider "virtualbox" do |vb|
   # vb.memory = "1024"

  config.vm.network :private_network, ip: "192.168.56.0"
        #   assigning private IP
        # jenkins.hostsupdater.aliases = ["development.local"]
  config.vm.synced_folder "install-jenkins", "/home/install-jenkins"
  config.vm.provision "shell", path: "./install-jenkins/provision.sh", privileged: false # for testing manual installation
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "install-jenkins.yaml"
   end
end