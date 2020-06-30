Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.box_version = "1905.1"
  config.vm.hostname = "generic"
  config.vm.synced_folder "./files", "/vagrant"

  config.vm.provision "ansible_local" do |ansible|
    ansible.limit = 'all'
    # ansible.inventory_path = 'hosts' #Come definisco gli host sulla VM? ¯\_(ツ)_/¯
    ansible.playbook = 'local.yml'
  end
end
