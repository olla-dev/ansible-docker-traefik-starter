# Apps playground
This includes DevSec's OS hardening playbooks (it will make a lot of changes to your server, USE AT YOUR OWN RISK)

## Services
* Portainer 
* Homer

## Requirements
* Install ansible

## Setup
* On your DNS, create a wildcard subdomain (e.g. apps.mydomain.com)
* Copy your ssh key to the ssh directory and set its permissions to 0600
* update provision.yml playbook
* update hosts file with your server IPs
* run ansible-galaxy install -r requirements.yml to install required playbooks

# Run 
```
ansible-playbook provision.yml
```