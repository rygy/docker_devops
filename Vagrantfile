# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  ## Kafka VM 1
  config.vm.define :kafka01 do |kafka01|
    config.vm.box = "ubuntu/trusty64"
    config.vm.hostname = "kafka-prod-01"
    config.vm.provision "ansible" do |ansible|
      ansible.playbook = "provisioning/playbook.yml"  
    end
  end

  ## Kafka VM 2
  config.vm.define :kafka02 do |kafka02|
    config.vm.box = "ubuntu/trusty64"
    config.vm.hostname = "kafka-prod-01"
    config.vm.provision "ansible" do |ansible|
      ansible.playbook = "provisioning/playbook.yml"
    end
  end
end
