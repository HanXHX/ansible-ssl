SSL management Ansible role
===========================
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-HanXHX.ssl-blue.svg)](https://galaxy.ansible.com/list#/roles/6420) [![Build Status](https://travis-ci.org/HanXHX/ansible-ssl.svg?branch=master)](https://travis-ci.org/HanXHX/ansible-ssl)

This role manages key/cert pairs. It checks modulus and deployment.

Requirements
------------

- On local machine, you need OpenSSL (available from PATH). LibreSSL can be managed (you can PR).

Role Variables
--------------

- `ssl_local_root_dir`: local root directory where you store your key/certs
- `ssl_local_cert_dir`: local directory where you store certificates
- `ssl_local_private_dir`: local directory where your store private key
- `ssl_root_dir`: remote root directory
- `ssl_cert_dir`: remote certificate directory
- `ssl_private_dir`: remote private key directory
- `ssl_pairs`: list of key pairs
- `ssl_notify`: handlers list (not used)

Dependencies
------------

None.

Example Playbook
----------------

See: [tests/test.yml](tests/test.yml).

Notes
-----

This role is developped mainly for Debian based systems. It _should_ work with all Linux/BSD OS. If you have some issue: you can PR with the offending vagrant box.

License
-------

GPLv2

Author Information
------------------

- Twitter: [@hanx\_hx](https://twitter.com/hanxhx_)

