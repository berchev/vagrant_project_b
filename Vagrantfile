Vagrant.configure("2") do |config|
  (1..2).each do |i|
    config.vm.define vm_name="web0#{i}" do |node|
      node.vm.box = "berchev/xenial64"
      node.vm.hostname = vm_name
    end
  end
  config.vm.provision "shell", path: "scripts/provision.sh"
end
  
