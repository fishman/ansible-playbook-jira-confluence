# Ansible Role: Sesam Backup

[![Build Status](https://travis-ci.org/fishman/ansible-role-sesam-backup.svg?branch=master)](https://travis-ci.org/fishman/ansible-role-sesam-backup)

Installs and configures Sesam Backup on RHEL/CentOS or Debian/Ubuntu servers.

## Requirements

No special requirements; note that this role requires root access, so either run it in a playbook with a global `become: yes`, or invoke the role in your playbook like:

    - hosts: database
      roles:
        - role: fishman.sesam_backup
          become: yes

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

This role was created in 2018 by [Reza Jelveh](https://reza.jelveh.me/)
