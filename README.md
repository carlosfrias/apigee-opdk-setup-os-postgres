Apigee OPDK Setup OS Postgres
=========

This role performs system updates that are required for the use of PostgreSQL as a part of an Apigee platform. 

Requirements
------------

This role requires elevated system privilege.

Role Variables
--------------

The collection `sysctl_pg` is used to perform systctl.conf updates specific for the use of PostgreSQL as a part of the 
Apigee platform.

    sysctl_pg:
    - { name: 'kernel.sem', value: "500 32000 32 1024" }
    


Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

Apache

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
<!-- BEGIN Google Required Disclaimer -->

# Not Google Product Clause

This is not an officially supported Google product.
<!-- END Google Required Disclaimer -->
<!-- BEGIN Google How To Contribute -->
# How to Contribute

We'd love to accept your patches and contributions to this project. Please review our [guidelines](CONTRIBUTION.md).
<!-- END Google How To Contribute -->
