metr1c
=========

This role installs metr1c vesion at /opt (the default way) and adds service to systemd.

Requirements
------------

Linux

Test now runs on ubuntu 22.04

Role Variables
--------------

`platform1c_version`: required version for installation (latest replaces in someting like 8.3.24.1323)
`platform1c_admin_user` 1c server user.
`platform1c_admin_pw`: password for the user.
`platform1c_admin_pw_path`: path to the (Ansible-encrypted) YAML file containing a password (see `molecule/default/secrets/`)

`metr1c_port`: localhost:port/metrics url part

Dependencies
------------

Installed platform1c role with RAC/RAS or working RAC/RAS on the server.

Example Playbook
----------------

See `molecule/default/coverge.yaml` for an example.

License
-------

GPLv3

Author Information
------------------

Danilkin Danila (MIPT) and Alexander Gorelyshev

Genlab, LLC

corvus-migratorius@proton.me
