# Ansible Servers

Vagrant.configure("2") do |config|

  config.vm.define "ansible_server_1", primary: true do |ansible_server_1|
    ansible_server_1.vm.box = "ubuntu/focal64"
    ansible_server_1.vm.box_check_update = false
    ansible_server_1.vm.hostname = "ansible-server-1"
    # ansible_server_1.vm.network "private_network", type: "dhcp"
    ansible_server_1.vm.network "private_network", ip: "172.28.128.3"
  end
  
  config.vm.define "ansible_server_2", autostart: false do |ansible_server_2|
    ansible_server_2.vm.box = "ubuntu/focal64"
    ansible_server_2.vm.box_check_update = false
    ansible_server_2.vm.hostname = "ansible-server-2"
    # ansible_server_2.vm.network "private_network", type: "dhcp"
    ansible_server_2.vm.network "private_network", ip: "172.28.128.4"
  end
  
  config.vm.define "ansible_server_3", autostart: false do |ansible_server_3|
    ansible_server_3.vm.box = "ubuntu/focal64"
    ansible_server_3.vm.box_check_update = false
    ansible_server_3.vm.hostname = "ansible-server-3"
    # ansible_server_3.vm.network "private_network", type: "dhcp"
    ansible_server_3.vm.network "private_network", ip: "172.28.128.5"
  end
  
  config.vm.define "ansible_server_4", autostart: false do |ansible_server_4|
    ansible_server_4.vm.box = "centos/8"
    ansible_server_4.vm.box_check_update = false
    ansible_server_4.vm.hostname = "ansible-server-4"
    # ansible_server_4.vm.network "private_network", type: "dhcp"
    ansible_server_4.vm.network "private_network", ip: "172.28.128.6"
  end  

end
