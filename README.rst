gitlab-packer
=============

Packer configurations for installing GitLab 6.0 on VMWare and Digital Ocean.

Inspired by/based on crashsystems' gitlab-docker_.

Usage
=====

* Edit lines 8-10 of *install_gitlab.sh*.
* If building for Digital Ocean, fill in the API key and client ID lines of *gitlab_digitalocean.json*.
* Run *packer build gitlab_vmware.json* or *packer build gitlab_digitalocean.json*

Notes
=====

* Building for Digital Ocean seems to have some reliability issues. The process may need to be run multiple times to get a working installation. A fix for this is in the works.

.. _gitlab-docker: https://github.com/crashsystems/gitlab-docker
