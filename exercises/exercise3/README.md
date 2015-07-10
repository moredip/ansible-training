# apache-centos

If the nodes aren't already up, you'll need to run:

	vagrant up node-1 node-2

### Topics covered

* playbook
* inventory
* initializing a role
* roles
* tagging
* templates


### General flow

Plain-old playbooks are not very re-usable.  So here we've taken the same concepts in the apache-paybook example and built an apache role.  

### Exercise

For this exercise, please ensure that the apache role is a part of the playbook.

Also, in the apache role template index.html.j2, make sure that the following
variable is included.

{{ ansible_hostname }}

### Commands

	ansible-playbook site.yml
