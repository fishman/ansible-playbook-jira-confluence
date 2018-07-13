# Jira / Confluence deployment

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

    ansible-galaxy install ansiblebit.oracle-java,5.14.12

## TODO
- [ ] fail2ban configuration
- [ ] partition layout
- [ ] nginx config
