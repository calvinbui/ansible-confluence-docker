[![Build Status](https://travis-ci.com/calvinbui/ansible-confluence-docker.svg?branch=master)](https://travis-ci.com/calvinbui/ansible-confluence-docker)

# Ansible Confluence Docker

Run Confluence inside a Docker container

##  Requirements

N/A

## Role Variables

`confluence_docker_tag`: Docker image tag to use found at https://hub.docker.com/r/atlassian/confluence-server/tags

`confluence_docker_data_dir`: Where to store data

## Dependencies

- Docker

## Example Playbook

```yaml
- hosts: servers
  become: true
  roles:
    - role: calvinbui.ansible_docker
    - role: calvinbui.ansible_confluence_docker
```

## License

GPLv3

## Author Information

http://calvin.me
