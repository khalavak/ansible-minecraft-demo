Copyright (C) 2014 Kim Halavakoski khalavakoski@gmail.com

# Building and deploying Minecraft server infrastructure with Ansible
These playbooks require Ansible => 1.8.2.

These playbooks have been created to automate the provisioning and deployment  
ff the Crosskey Banking Solutions server infrastructure 

Have a look at the Ansible documentation before proceeding: 
http://docs.ansible.com/intro.html

The Ansible configurations, playbooks and structure follow the best practices 
documented here as much as possible: 

http://docs.ansible.com/playbooks_best_practices.html

# Demo
A video of the Ansible playbook run can be found here:

https://vimeo.com/121509055


# Infrastructure

The infrastructure consists of multiple servers running Ubuntu Linux. 
The inventory is documented in the following files in the /inventory 
directory:

    $ ls inventory/
    ec2_control
    minecraft_servers

The ec2_control inventory contains references to localhost at the AWS commands
are run from localhost to AWS API.

The minecraft_servers inventory is populated with the AWS EC2 instances that
are provisioned and deployed in the Ansible playbooks.

The following commands must be run to first provision the EC2 instancers in
AWS and then deploy the configurations on the EC2 instances. I have separated
these into two separate playbooks for clarity but all actions could be done
in the same playbook.

    $ ansible-playbook -i inventory/ec2_control minecraft_provision.yml
    $ ansible-playbook -i inventory/minecraft_servers minecraft_deploy.yml


This could be tested on vagrant instances first but this is something I have 
left out from these playbooks.

# References
For more infromation on Vagrant see here : 

https://docs.vagrantup.com/v2/why-vagrant/index.html
https://julien.ponge.org/blog/scalable-and-understandable-provisioning-with-ansible-and-vagrant/
http://hakunin.com/six-ansible-practices#automate-adding-your-pub-key-to-vms

