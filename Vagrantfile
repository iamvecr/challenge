Vagrant.configure("2") do |config|
  # config.vm.box = "centos/7"
  # config.vm.box_version = "1905.1"
  # config.vm.hostname = "generic"
  # config.vm.synced_folder "./files", "/vagrant"
  #
  # config.vm.provision "ansible" do |ansible|
  #   ansible.verbose = 'v'
  #   ansible.limit = 'all'
  #   ansible.inventory_path = '/etc/ansible/hosts' #Come definisco gli host sulla VM? ¯\_(ツ)_/¯
  #   ansible.playbook = 'docker.yml'
  # end

  config.vm.provision "ansible_local" do |ansible|
    ansible.limit = 'all'
    ansible.inventory_path = 'hosts'
    ansible.playbook = "docker.yml"
     ansible.galaxy_command = "ansible-galaxy install nickjj.docker"
  end



  # config.vm.provision "shell", inline: "echo Hello"

  config.vm.define "vm1" do |vm1|
    config.vm.box = "centos/7"
    config.vm.box_version = "1905.1"
    config.disksize.size = '50GB'
    config.vm.hostname = "vm1"
  end

  config.vm.define "vm2" do |vm2|
    config.vm.box = "centos/7"
    config.vm.box_version = "1905.1"
    config.disksize.size = '50GB'
    config.vm.hostname = "vm2"
  end
end
