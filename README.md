ansible-git-common
=====

This role installs from source Git, a distributed version control system,
on any RHEL/CentOS and Debian Linux system.

Requirements
------------

This role requires Ansible 1.4 or higher and platform requirements are listed
in the metadata file.

Role Variables
--------------

The variables that can be passed to this role and a brief description about
them are as follows.

    # The version to install
    git_version: '1.8.5.5'


Examples
========

1) Install latest git version

    - hosts: all
      roles:
      - ansible-git-common


2) Install specific git version

    - hosts: all
      roles:
      - {role:        'ansible-git-common',
         git_version: '1.8.5.5'}

Dependencies
------------

None

License
-------

BSD

Author Information
------------------

Parv Mihai

