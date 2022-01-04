# Ansible Role: docker-wordpress

Ansible role to setup wordpress site using docker container

## Requirements

CentOS 7 

## Sample Playbook

`playbook.yml`

    - hosts: prod
      roles:
        - wordpress
      vars:
        install_ansible_packages: true
      become: true
      
`hosts`

    [wordpress]
    localhost

Running ansible playbook:

    ansible-playbook -i hosts.yaml playbook.yaml

