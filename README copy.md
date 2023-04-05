# AIDE

An Ansible role that installs AIDE to CENTOS 7/8, Rocky9 and Ubuntu. More info about AIDE: [link](https://aide.github.io/)


## Requirements

Make sure, you made your vars file with valid path to custom template or you can use Default vars.

You need `ansible 2.13.7` to run this module

## Tasks descriptions

- main.yml - Run the OS check and run the relevant playbook
- configure_aide.yml - Configure AIDE
- install_el7.yml - Deploy AIDE on Rhel7.x
- install_el8.yml - Deploy AIDE on Rhel8.x
- install_ubuntu.yml - Deploy AIDE on Ubuntu


## Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
- hosts: servergroup
  become: true
  become_user: lee

  vars_files:
    - vars/main.yml
    
  roles:
    - nerve4-aide
```

## Maintainer Information
Lee | 2023