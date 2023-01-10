# Commands

## run normal commands
`ansible-playbook run.yaml`

## run commands against tags
`ansible-playbook --tags="port,containers" run.yml`

## Setup - Install requirements
`ansible-galaxy install -r requirements.yml`

## Secrets
`ansible-vault create host_vars/YOUR_HOSTNAME/secret.yml`

`ansible-vault edit host_vars/YOUR_HOSTNAME/secret.yml`

Add this line to the play to avoid loggin secrets to command line

`no_log: True`

## Run with passwords
`ansible-playbook --ask-become-pass -e@passwords.yaml run.yaml`

## Create role 
`ansible-galaxy role init kvm_provision`