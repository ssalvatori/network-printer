Vagrant.configure('2') do |config|
 
    config.vm.box = "bento/debian-12.5"
    config.vm.hostname = 'printer'

    config.vm.network :forwarded_port, guest: 631, host: 1631

    config.vm.provision "ansible" do |ansible|
        ansible.compatibility_mode = "2.0"
        ansible.playbook = "main.yml"
    end

end
