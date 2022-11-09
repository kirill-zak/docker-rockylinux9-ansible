# Rocky Linux 9 Ansible test image
Rocky Linux 9 docker container for Ansible playbook and role testing.

## Tags

  - `latest`: Latest stable version of Rocky Linux 9 with built-in Ansible

## How to Build

To build the image on your own locally, do the following:

  1. [Install Docker](https://docs.docker.com/engine/installation/).
  2. `cd` into this directory.
  3. Run `docker build -t docker-rockylinux9-ansible .`


## How to Use

  1. [Install Docker](https://docs.docker.com/engine/installation/).
  2. Pull pre-build image via `docker image pull kirillzak/docker-rockylinux9-ansible:latest` or build image via `docker build -t docker-rockylinux9-ansible .`
  3. Run a container from the image: `docker run --detach --privileged --volume /sys/fs/cgroup:/sys/fs/cgroup:ro docker-rockylinux9-ansible:latest`

## Author

[Kirill Ziuzin](https://kirill-zak.ru/)

## Thanks

Based on ideas of [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).