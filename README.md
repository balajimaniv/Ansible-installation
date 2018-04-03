# Ansible-installation
This is a first sample project with ansible installation 

## Install Ansible on Redhat

### commands to execute
    *  rpm -Uvh https://dl.fedoraproject.org/pub/epel/epel-release-latest-7.noarch.rpm

    *  yum -y install ansible
    
    *  ansible --version


## create file webserver-httpd.yml and save below content
```python
   - hosts: localhost
  tasks:
    - name: install httpd
      yum: name=httpd update_cache=yes state=latest
```
### Note: since its python be carefull with intendation

## execute ansible playbooks
 ansible-playbook webserver-httpd.yml
 
 The above command will excute the plays written in playbooks.

    





Reference:

https://developers.redhat.com/blog/2016/09/02/how-to-install-and-configure-ansible-on-rhel/


