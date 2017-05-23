# Docker

Docker and Docker Compose role installation for
[Dalee/ubuntu](https://atlas.hashicorp.com/Dalee/boxes/ubuntu/).

Service is disabled by default. Having active docker0 bridge
could interfere with NFS mounts IP guess by Vagrant.

Just use `sudo systemctl start docker` to run when needed.

# Insecure registry

Provide var `docker_insecure_registry` in vagrant.yml inventory
in order to allow insecure registry access for docker daemon.

```
- hosts: localhost
  ...
  vars:
    - docker_insecure_registry: docker-registry.example.com:80
```
