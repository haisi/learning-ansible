# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  # The most common configuration options are documented and commented below.
  # For a complete reference, please see the online documentation at
  # https://docs.vagrantup.com.

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://vagrantcloud.com/search.
  config.vm.box = "ubuntu/jammy64"

#   config.ssh.username = "ubuntu"
#   config.ssh.password = "ubuntu"

  config.vm.provider "virtualbox" do |v|
      v.gui = true
      v.memory = 2048
      v.customize ['modifyvm', :id, '--clipboard', 'bidirectional']
  end

  # Currently "ubuntu/bionic64" on VirtualBox requires `type: "virtualbox"`
  # to make synced folder works.
  config.vm.synced_folder ".", "/vagrant", type: "virtualbox"

#   config.vm.provision :shell, inline: "sudo apt-add-repository -y multiverse"
  # Update repositories
#   config.vm.provision :shell, inline: "sudo apt update -y"

  # Upgrade installed packages
#   config.vm.provision :shell, inline: "sudo apt upgrade -y"

#   config.vm.provision "shell", path: "install-desktop.sh"

# sudo apt-get install virtualbox-guest-additions-iso
# sudo mkdir /media/vbox
# sudo mount -o loop /usr/share/virtualbox/VBoxGuestAdditions.iso /media/vbox
# sudo /media/vbox/VBoxLinuxAdditions.run

  # Add desktop environment
#   config.vm.provision :shell, inline: "sudo apt install -y --no-install-recommends ubuntu-desktop"
#   config.vm.provision :shell, inline: "sudo apt install -y build-essential dkms"
#   config.vm.provision :shell, inline: "sudo apt install -y --no-install-recommends virtualbox-guest-dkms virtualbox-guest-utils virtualbox-guest-x11"
#   config.vm.provision :shell, inline: "sudo apt install -y --no-install-recommends virtualbox-guest-utils virtualbox-guest-x11"
#   config.vm.provision :shell, inline: "sudo apt-get install -y virtualbox-guest-additions-iso"
  # Add `vagrant` to Administrator
#   config.vm.provision :shell, inline: "sudo usermod -a -G sudo vagrant"

#   # Add Google Chrome
#   config.vm.provision :shell, inline: "sudo apt install -y google-chrome-stable"

#   # Add Chromium
#   config.vm.provision :shell, inline: "sudo apt install -y chromium-browser"

#   # Add Firefox
#   config.vm.provision :shell, inline: "sudo apt install -y firefox"

  # Restart
#   config.vm.provision :shell, inline: "sudo shutdown -r now"

#   config.vm.provision "ansible" do |ansible|
#     ansible.playbook = "my-playbook.yml"
#   end
  # Disable automatic box update checking. If you disable this, then
  # boxes will only be checked for updates when the user runs
  # `vagrant box outdated`. This is not recommended.
  # config.vm.box_check_update = false

  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine. In the example below,
  # accessing "localhost:8080" will access port 80 on the guest machine.
  # NOTE: This will enable public access to the opened port
  # config.vm.network "forwarded_port", guest: 80, host: 8080

  # Create a forwarded port mapping which allows access to a specific port
  # within the machine from a port on the host machine and only allow access
  # via 127.0.0.1 to disable public access
  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  # config.vm.network "private_network", ip: "192.168.33.10"

  # Create a public network, which generally matched to bridged network.
  # Bridged networks make the machine appear as another physical device on
  # your network.
  # config.vm.network "public_network"

  # Share an additional folder to the guest VM. The first argument is
  # the path on the host to the actual folder. The second argument is
  # the path on the guest to mount the folder. And the optional third
  # argument is a set of non-required options.
  # config.vm.synced_folder "../data", "/vagrant_data"

  # Provider-specific configuration so you can fine-tune various
  # backing providers for Vagrant. These expose provider-specific options.
  # Example for VirtualBox:
  #
  # config.vm.provider "virtualbox" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
  #   vb.gui = true
  #
  #   # Customize the amount of memory on the VM:
  #   vb.memory = "1024"
  # end
  #
  # View the documentation for the provider you are using for more
  # information on available options.

  # Enable provisioning with a shell script. Additional provisioners such as
  # Ansible, Chef, Docker, Puppet and Salt are also available. Please see the
  # documentation for more information about their specific syntax and use.
  # config.vm.provision "shell", inline: <<-SHELL
  #   apt-get update
  #   apt-get install -y apache2
  # SHELL
end
