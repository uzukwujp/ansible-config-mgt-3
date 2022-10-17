

## ANSIBLE DYNAMIC ASSIGNMENTS (INCLUDE) AND COMMUNITY ROLES

Project 14 builds on what we learnt in project 13 and introduces us to another feature *Include*.

### INCLUDE
Include does similar thing as *Imports* but differs because it is dynamic. Dynamic in the sense that ansible is able pick changes in playbooks added to a master playbook in real time. In import ansible preprocesses everything runs the playbook with the data it has. Changes made while executing the playbook is ignored.

### BEST USE OF INCLUDE
Include is best suited for feeding environment variables to ansible.

- Note for most part stick with *Import* statement as *Include* can make debugging difficult.
