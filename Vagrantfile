Vagrant.configure("2") do |config|
    config.vm.box = "astralinux-test"
    config.vm.guest = "debian"
    config.ssh.shell = "bash"

    config.vm.define "ipaserver" do |ipa|
        ipa.vm.provider "virtualbox" do |vb|
            vb.name = "v_ipaserver"
            vb.memory = 4096
            vb.cpus = 3
        end
        ipa.vm.hostname = "ipaserver.test.local"
        ipa.vm.network "forwarded_port", guest: 80, host: 8080   
    end

    config.vm.define "ipaclient" do |ipa|
        ipa.vm.provider "virtualbox" do |vb|
            vb.name = "v_ipaclient"
            vb.memory = 3072
            vb.cpus = 2
        end
        ipa.vm.hostname = "ipaclient.test.local"
        ipa.vm.network "forwarded_port", guest: 80, host: 8081     
    end

    config.vm.define "zabbix" do |zbx|
        zbx.vm.provider "virtualbox" do |vb|
            vb.name = "v_zabbix"
            vb.memory = 2048
            vb.cpus = 2
        end
        zbx.vm.hostname = "zabbix.test.local"
        zbx.vm.network "forwarded_port", guest: 80, host: 8082     
    end


end