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

# Dependencies

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

# Example Playbook

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - raveshaww.docker_ce

# License
-------

BSD

# Author Information

This role was created in 2023 by [Austin Clark](https://github.com/Raveshaww). 
