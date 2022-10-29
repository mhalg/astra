# I used yandex cloud VM for verification of ipaserver installation and I've set hostname manually "sudo hostnamectl set-hostname ipaserver.test.local", but for Vagrant scenario it should be set automatically by Vagrant VM setup
adjust ipaserver ip in ./hosts file
use following command to setup ipaserver:
ansible-playbook freeipa_playbook.yml
