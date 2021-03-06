Ansible is an IT automation tool. It can configure systems, 
deploy software, and orchestrate more advanced IT tasks
 such as continuous deployments or zero downtime rolling updates.

Basic Concepts
---------------
Control Node - Server from where you run Ansible Commands/Scripts/playbooks.
Manage Node - servers you managed/controlled by Ansible.
Inventory - A list of managed nodes. 
Modules - The units of code Ansible executes.
Tasks - The units of action in Ansible. 
Playbooks - Ordered lists of tasks, saved so you can run those tasks in that order repeatedly.

you cannot use a Windows machine as a control node.

default conf files
--------------------
/etc/ansible/hosts
/etc/ansible/ansible.cfg

Priorities of ansible conf files
----------------------------------
1) ANSIBLE_CONFIG (environment variable if set)
2) ansible.cfg (in the current directory)
3) ~/.ansible.cfg (in the home directory)
4) /etc/ansible/ansible.cfg

Note - Ansible will not automatically load a config file 
from the current working directory if the directory is world-writable.

2-Way to run ansible
---------------------
1) Ad-hoc command
2) Playbook 