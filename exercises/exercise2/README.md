# apache_playbook

If the nodes aren't already up, you'll need to run:

	vagrant up node-1 node-2


### Topics covered

* Inventory
* Creating a playbook.
* Using vars
* Using with_items
* Using host ranges

### General flow

Configuring systems with ad-hoc tasks can be annoying -- and ad-hoc tasks don't really keep a good record of how a system ***should*** be configured.

### Exercise

In the playbook for this exercise, please ensure that httpd is installed on the
target host.


Then, in this example, we show how to use a simple playbook
to setup Apache on 2 hosts by running the following command.

	ansible-playbook site.yml
