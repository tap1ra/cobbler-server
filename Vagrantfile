Vagrant.configure(2) do |config|
  config.vm.box = "CentOS6.6_Packer"
  config.vm.hostname = "cobbler-server"
  config.vm.network :private_network, ip: "192.168.20.2", virtualbox__intnet: "cobbler-net"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
    ansible.limit = "all"
  end
end
