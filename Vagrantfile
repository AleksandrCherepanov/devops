# -*- mode: ruby -*-
# vi: set ft=ruby :
hosts = {
    "192.168.77.10" => "n1",
    "192.168.77.11" => "n2"
}

Vagrant.configure("2") do |config|
    config.ssh.insert_key = false
    config.ssh.forward_agent = true
    check_guest_additions = false
    functional_vboxsf = false

    config.vm.box = "bento/ubuntu-20.04"
    hosts.each do |ip, name|
        config.vm.define name do |machine|
            machine.vm.hostname = name

            if name == "n1" then
                machine.vm.network "forwarded_port", guest: 8001, host: 8123
            end

            machine.vm.network :private_network, ip: ip,
                virtualbox__intnet: true

            machine.vm.provider "virtualbox" do |v|
                v.memory = 512
                v.cpus = 1
            end
        end
    end
end