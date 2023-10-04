[![CI](https://github.com/Raveshaww/ansible-role-docker-ce/actions/workflows/ci.yml/badge.svg)](https://github.com/Raveshaww/ansible-role-docker-ce/actions/workflows/ci.yml)
# Ansible Role: Docker CE

A simple role to install the following packages on Debian, Fedora, and Ubuntu systems:
- docker-ce
- docker-ce-cli
- containerd.io
- docker-buildx-plugin
- docker-compose-plugin

Additionally, on Debian and Ubuntu systems: 
- curl
- ca-certificates
- gnupg

Additionally, on Fedora systems:
- dnf-plugins-core

This role should work as is for CentOS and RHEL systems, though it has not been tested.

# Requirements

No requirements.

# Role Variables

The variables listed within the vars folder note which packages will be installed. In the case of Debian based systems, this will also indicate the repo to be added. In the case of Fedora, the repos added are noted in templates/docker-ce.j2

# Example Playbook


    - hosts: servers
      roles:
         - raveshaww.docker_ce

# License
-------

BSD

# Author Information

This role was created in 2023 by [Austin Clark](https://github.com/Raveshaww). 
