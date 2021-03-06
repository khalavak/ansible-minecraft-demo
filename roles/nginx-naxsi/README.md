Role: nginx-naxsi
=================

NAXSI is an open source, high performance, low rules maintenance, Web Application Firewall for nginx. This role manages the base installation and configuration of 'nginx-naxsi' and makes 
sure that the service is running and that the configurations follow the           
standard set in this role.  

NOTE: This role does not setup any specific website content files or web-applications
and those has to be defined, installed and configured using a separate role.
See the 'entrant' role for an example.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: webservers
      roles:
        - nginx-naxsi

License
-------

BSD

Author Information
------------------

Author: Kim Halavakoski <khalavakoski@gmail.com>
Company: Deductive Labs Ab Ltd.
Web: http://www.deductivelabs.com

