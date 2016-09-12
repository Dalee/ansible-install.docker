# Dalee Tech

Docker and Docker Compose role installation for Debian based distributions.
Currently used internally for Vagrant environment.


Provide var `docker_insecure_registry` in vagrant.yml inventory in
 order to allow insecure registry access for docker daemon.

```
- hosts: localhost
  ...
  vars:
    - docker_insecure_registry: docker-registry.example.com:80
```