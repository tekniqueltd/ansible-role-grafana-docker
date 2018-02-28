Ansible Role: grafana-docker
=========

Ansible role for deploying Grafana using docker and docker-compose.

Requirements
------------

- Debian 9+
- Ubuntu 16.04+ (untested)

Requirements
------------

- Ansible 2.4+ (on execution host)
- Docker 17+ (on remote host)

Role Variables
--------------

See `./defaults/main.yml` for configurable variables and their defaults


Example Playbook
----------------

    ---
    - hosts: servers
      roles:
         - { role: grafana-docker, 
             grafana_docker_admin_pass: password, 
             grafana_docker_expose_port: 3000 
           }


Add as a submodule to your playbook repo
----------------------------------------

    git submodule add https://github.com/teknique/ansible-role-grafana-docker.git roles/grafana-docker

