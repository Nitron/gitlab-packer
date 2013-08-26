gitlab-packer
=============

Build GitLab images/snapshots for VMWare and Digital Ocean

Usage
=====

* Edit lines 8-10 of *install_gitlab.sh*.
* If building for Digital Ocean, fill in the API key and client ID lines of *gitlab_digitalocean.json*.
* Run *packer build gitlab_vmware.json* or *packer build gitlab_digitalocean.json*
* If building for VMWare, go through the OS installation process manually. Packer will take over after Ubuntu is installed. Be sure to install the OpenSSH server.

Notes
=====

* A preseed configuration for building with VMWare is in the works.
* Building for Digital Ocean seems to have some reliability issues. The process may need to be run multiple times to get a working installation. A fix for this is also in the works.