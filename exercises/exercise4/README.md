# apache-centos-ubuntu

If the nodes aren't already up, you'll need to run:

	vagrant up node-1 node-2 node-3

### Topics covered

* playbook
* inventory
* roles
* tagging
* include_vars
* conditionals
* seperate task files
* host_vars

### General Flow


We're adding a new node this time, and it just so happens to be an Ubuntu node.  Now that's going to require some changes to our role.

We are also showing how to use host_vars to override the apache_test_message default.

No problem though, we still run the playbook in the same way.

### Exercise

In this exercise, let's make sure that the role installs based on the facts
included for the ansible_os_family(i.e. RedHat or Debian).

Then make sure the proper template is applied for httpd.conf.j2 in the main
playbook.

### Commands

You can use this command to check your work:
	ansible-playbook site.yml --syntax-check

	ansible-playbook site.yml
