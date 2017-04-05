uclalib_role_epel [![Build Status](https://travis-ci.org/UCLALibrary/uclalib_role_epel.svg?branch=master)](https://travis-ci.org/UCLALibrary/uclalib_role_epel)
=========

This Ansible role installs the EPEL repository so that Yum can use it.

Role Variables
--------------

There is one default variables for this role that can be overridden if needed:

    epel_url: https://dl.fedoraproject.org/pub/epel/epel-release-latest-6.noarch.rpm


Example Playbook
----------------

A simple example playbook that overrides a default variable:boom

    ---
    
    - hosts: all
    
    # Optionally, use a different EPEL repository location
    - epel_url: https://mirrors.kernel.org/fedora-epel/6/x86_64/epel-release-6-8.noarch.rpm
    
    roles:
      - { role: uclalib_role_epel }

License
-------

BSD 3-Clause

Author Information
------------------

For more information about this role contact its author, [Anthony Vuong](https://github.com/avu0ng).
