# common_role

If you haven't done so already:

	vagrant up node-1 node-2 node-3 haproxy

This brings up another node.  


### Topics Covered

* looping with array of dictionaries for user information
* using a common role
* inventory groups and child groups
* roles
* tagging
* include_vars
* conditionals
* separate task files
* using group_vars to set the remote user
* including playbooks within playbooks
* using host ranges
* using registered variables

### Exercise

In this exercise, let's include the nested playbook app.yml inside of site.yml

Also, review how the rest of the playbook run is going to occur by reading the 
playbook.

### General flow

* Add a new haproxy role
* update the playbook to use the common role

### Commands

	ansible-playbook site.yml
