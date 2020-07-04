Vagrant.configure("2") do |config|

  config.vm.provision "ansible_local" do |ansible|
    ansible.limit = 'all'
    ansible.inventory_path = 'hosts'
    ansible.galaxy_role_file = "requirements.yml"
    ansible.playbook = 'docker.yml'
  end

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
