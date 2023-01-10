# Commands

## run normal commands
ansible-playbook run.yaml

## run commands against tags
ansible-playbook run.yml --tags="port,containers"

## Run with passwords
ansible-playbook run.yaml --ask-become-pass -e@passwords.yaml

## Setup - Install requirements
ansible-galaxy install -r requirements.yml

## create secrets
ansible-vault create host_vars/YOUR_HOSTNAME/secret.yml
ansible-vault edit host_vars/YOUR_HOSTNAME/secret.yml
    no_log: True
## Create role 
ansible-galaxy role init kvm_provision