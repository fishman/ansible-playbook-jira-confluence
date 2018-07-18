# Jira / Confluence deployment
[![Build Status](https://travis-ci.org/fishman/ansible-playbook-jira-confluence.svg?branch=master)](https://travis-ci.org/fishman/ansible-playbook-jira-confluence)

## Installing recent ansible

On RHEL and CentOS

    sudo yum install ansible

On Ubuntu

    sudo apt-get update
    sudo apt-get install software-properties-common
    sudo apt-add-repository ppa:ansible/ansible
    sudo apt-get update
    sudo apt-get install ansible

## Oracle JDK on JIRA / Confluence servers

JIRA / Confluence don't work with OpenJDK and require Java 8. Newer versions of the ansiblebit role only support Java 9.


## Enabling the corporate proxy

You can add a corporate proxy by setting the environment information in group_vars/proxy

    proxy_env:
      http_proxy: http://proxy:8080
      https_proxy: http://proxy:8080

## Sesam Backup integration

-- http://wiki.sep.de/wiki/index.php/SEP_Sesam_Scripts#Ansible 

## TODO
- [ ] fail2ban configuration
- [ ] system hardening
- [x] partition layout
- [x] nginx config
