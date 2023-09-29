Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.network "private_network", type: "dhcp"
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
    vb.cpus = 2
  end

  # Defina o nome do host
  config.vm.hostname = "meu-host-ubuntu"

  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    # Personalize sua máquina virtual aqui
  SHELL
end
