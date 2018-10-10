# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
    config.vm.box = "ubuntu/xenial64"
    config.vm.hostname = "docker-host"
    config.vm.provision "docker"
    config.vm.synced_folder '/host/path', '/guest/path', SharedFoldersEnableSymlinksCreate: false
end


# docker run -it --rm -v $(pwd)/.vagrant/machines/test-2018-10-09/virtualbox/private_key:/root/.ssh/private_key  -v /home/danielbascon/ansible/ansible-wso2apim/tests:/devops/source chakray/platform:1.0.0 bash