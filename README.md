Update Haproxy Configuration
=========

This role can be used to configure an already installed haproxy instance.
It is designed to configure rather simple haproxy sidecar instances with straight-forward configurations.
You can always use a different template, of course.

[![Build Status](https://travis-ci.org/Rheinwerk/ansible-role-update_haproxy_config.svg?branch=master)](https://travis-ci.org/Rheinwerk/ansible-role-update_haproxy_config)

Requirements
------------

Installed haproxy.

Role Variables
--------------

There is one main variable that drives this role: `_update_haproxy_config`. It is a map that contains all configuration and settings for this role.
Please see `defaults/main.yml` for details.

Dependencies
------------

None.


Example Playbook
----------------

The general contract of this role is to take the variables map `_update_haproxy_config` from `defaults/main.yml` as a template for your configuration and pass that configuration as a parameter to this role.

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      var:
        HAPROXY_CONFIG:
          ...
      roles:
         - { role: update_haproxy_config, tags: [ 'haproxy' ] _update_haproxy_config: "{{ HAPROXY_CONFIG }}" }
License
-------

Please see LICENSE.

Author Information
------------------

Original author is [Daniel Schneller](https://github.com/dschneller) as member of the [Rheinwerk](https://github.com/Rheinwerk) project.

