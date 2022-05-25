

## ANSIBLE DYNAMIC ASSIGNMENTS (INCLUDE) AND COMMUNITY ROLES

Project 13 builds on what we learnt in [project 12](https://github.com/uzukwujp/ansible-config-mgt-2)  and introduces us to another feature *Include*.

### INCLUDE
Include does similar thing as *Imports* but differs because it is dynamic. Dynamic in the sense that ansible is able pick changes in playbooks added to a master playbook in real time. In import ansible preprocesses everything runs the playbook with the data it has. Changes made while executing the playbook is ignored.

### BEST USE OF INCLUDE
Include is best suited for feeding environment variables to ansible.

- Note for most part stick with *Import* statement as *Include* can make debugging difficult.








![project-13-apache2 running on lb](https://user-images.githubusercontent.com/52359007/170307139-735efe03-ff3f-4c9b-8ed6-5e777328edbb.PNG)







![project-13-nginx-running-in-uat-env](https://user-images.githubusercontent.com/52359007/170307169-73485083-0409-482c-b9ab-c5600593c28e.PNG)


## When condition

Another important feature in this project is the when condition. It was used to decide the nature of load balancer installed in an environment depending on which variables is set to true

see the code snippet below for better understanding:


![when](https://user-images.githubusercontent.com/52359007/170379820-396cb3f5-ed4b-4f77-8090-3e2b767dd59e.PNG)


See the different load balancers installed sucessfully below:



![project-13-apache2 running on lb](https://user-images.githubusercontent.com/52359007/170380011-66b035b6-babd-4591-b0b4-7d9520adf01f.PNG)




![project-13-nginx-running-in-uat-env](https://user-images.githubusercontent.com/52359007/170380046-b0735dc5-eca2-4b8e-9cb6-8d187a52a854.PNG)
