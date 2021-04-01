# Docker Setup & Launching httpd Webserver

## System Requirements
These roles have only been tested with:
* RedHat Linux `8`,`7`
* Ansible version:
  * `2.10.3`

In addition, the roles specifically target the `RedHat OS` family, including `CentOS` and `Amazon Linux`, and may not function for other host OS's.

## Description
Contains two roles:
* `docker-setup` : Configure docker environment in target node(s).
* `httpd-server-docker` : Configure httpd webserver.

## Prerequisite
Require Ansible version 2.10.3 installed.

## Getting Started
### Steps:
* Put target node IP in inventory file i.e host
```yaml
[docker_host]
ip  ansible_user=root ansible_ssh_pass=pass ansible_connection=ssh
```
* We can give any port we like, just need to edit the vars file `/roles/httpd-server-docker/vars/main.yml`
```yaml
port_for_httpd_svc: "3898"
``` 
* Run playbook
```bash
ansible-playbook setup.yml
```
### Connect me
* [Linkedin](https://linkedin.com/in/rahulkumar-choudhary "Rahulkumar Choudhary")
* [Twitter](https://twitter.com/Rahulkumar29420 "Rahulkumar29420")
* [Medium](https://rahulchoudhary5768.medium.com/ "Rahulkumar Choudhary")
