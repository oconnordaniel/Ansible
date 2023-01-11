# Ansible
Home for all my ansible plays and roles. Mostly for managing my homelab.


# Playbooks

- Updates
- Setup desktop
- Setup server
- Setup hypervisor
- Setup Docker host
- Setup file server

Plays: 
- updates
- server packages
- desktop packages / terminal 
- security
    - ssh keys
    - users and passwords
    - nagios agent

Apps: 
- website
- mastodon
- nagios
- dns server

# Setup

## Setup python and ansible

```
sudo {{ package manager }} install python3 python3-pip python3-venv
python3 -m venv ansible
source ansible/bin/activate
python3 -m pip install ansible
```

## Gen SSH keys to be used

```
ssh-keygen -t ed_25519 -C ansible-key -f ./files/id_ed25519_ansible
cat ./files/id_ed25519_ansible.pub >> plays/roles/ssh/files/authorized_keys 
```