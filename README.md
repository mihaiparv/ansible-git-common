ansible-git-common
=====

This role installs Git, a distributed version control system, on any RHEL/CentOS and Debian Linux system.

Requirements
------------

This role requires Ansible 1.4 or higher and platform requirements are listed
in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows.

    # The version to install
    git_version: '1:1.9.0-1~ppa0~precise1'


Examples
========

1) Install git with default settings

    - hosts: all
      roles:
      - ansible-git-common


2) Install specific git version for Ubuntu systems

    - hosts: all
      roles:
      - {role: ansible-git-common,
         git_version: '1:1.9.0-1~ppa0~precise1'}

2) Install specific git version for RHEL/CentOS systems

    - hosts: all
      roles:
      - {role: ansible-git-common,
         git_version: '1.7.1'}

Dependencies
------------

None

License
-------

BSD

Author Information
------------------

Parv Mihai

