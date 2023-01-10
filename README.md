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

`sudo {{ package manager }} install python3 python3-pip python3-venv` 

`python3 -m venv ansible`

`source ansible/bin/activate`

`python3 -m pip install ansible`
