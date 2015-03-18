Role Name: ansible
==================

This role installs and setups ansible on the target server and downloads
the Deductive Labs ansible repository from Bitbucket.


Requirements
------------

There are no pre-requisites to this role. Everything will be i
installed on the server with this role


Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

This role has the following dependencies:

- Entrant - This role is dependent on Entrant role for generation and 
  provisioning of Entrant guests into the Freeradius database tables


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: server
      roles:
         - ansible

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
