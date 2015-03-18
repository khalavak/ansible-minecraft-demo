Ansible Role: update
=====================

This role simply updates the system with the latest system and application
updates via aptitude / apt-get

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.


Role Variables
--------------

The role does not use any variables but the tasks use the following tags: update & upgrade
The tags can be used to run just an update or upgrade of system applications.


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - update

Furthermore, the tags can be used to specify specific tasks:
ansible-playbook -i inventory/production_servers_ --skip-tags upgrade


License
-------

BSD

Author Information
------------------
Kim Halavakoski <khalavakoski@gmail.com>
Copyright (C) 2013 Deductive Labs Ab Ltd.
