Vagrant.configure("2") do |config|
    config.vm.box = "astralinux-test"
    config.vm.guest = "debian"
    config.ssh.shell = "bash"

    config.vm.define "ipaserver" do |ipa|
        ipa.vm.provider "virtualbox" do |vb|
            vb.name = "v_ipaserver"
        end
        ipa.vm.hostname = "ipaserver.test.local"
    end


end