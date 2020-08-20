# samba_fedora_server_ansible

This ansible script install on remote machine The samba server

To install samba run:

ansible-playbook -vv -i hosts site.yaml

To uninstall samba run:

ansible-playbook -vv -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade package samba

For example, to launch only task regarding upgrade os, run:

ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
