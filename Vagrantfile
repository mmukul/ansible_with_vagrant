
## Vagrant second box ##

Vagrant.configure(2) do |config|
config.vm.box = "centos/7"
 config.vm.network "private_network", ip: "192.168.33.10"
 config.vm.provision "ansible" do |ansible|
  ansible.inventory_path = "/etc/ansible/hosts"
  ansible.playbook = "/etc/ansible/playbook/ansible/vagrant_playbook_example.yml"
  ansible.verbose = "-vv"
  ansible.sudo = true
  ansible.limit = 'all'
end
 end
