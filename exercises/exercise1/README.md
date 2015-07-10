# ad-hoc examples

### Topics Covered

* ansible installation methods
* ad-hoc ansible
* command-line options: ```-i -u -m -a```
* using ansible.cfg


### General flow


Bring up the VMs by running the following command:

	vagrant up node-1 node-2

Add the vagrant ssh key:

	ssh-add ~/.vagrant.d/insecure_private_key


### Commands

Install ansible with pip, but explain other methods (brew, yum, apt, etc)

	pip install ansible

Run the following commands and experiment:

	ansible web -i inventory/hosts -u vagrant -m setup
	
	ansible web -i inventory/hosts -u vagrant -m yum -a "name=httpd state=present" -s

Specifying the inventory and user is annoying, so open up ansible.cfg and uncomment the entries for inventory and remote_user.

	
	ansible web -m service -a "name=httpd state=started" -s
	
	ansible web -m service -a "name=httpd state=stopped" -s
	
	ansible web -m yum -a "name=httpd state=absent" -s
	
	
Imagine the calories saved by less typing.
