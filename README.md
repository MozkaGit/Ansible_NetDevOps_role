[![Push to Galaxy](https://github.com/MozkaGit/Ansible_NetDevOps_role/actions/workflows/push_to_galaxy.yml/badge.svg)](https://github.com/MozkaGit/Ansible_NetDevOps_role/actions/workflows/push_to_galaxy.yml)

Role Name
=========

1. Replace Interface Configuration: It replaces the device configuration for specified interfaces, enabling them and setting their descriptions. This is done for both WAN and LAN interfaces.

2. Configure IP Routes: After configuring the interfaces, the playbook configures IP routes on the routers based on the router's hostname

3. Execute Commands: The playbook runs several commands on the routers using the `cisco.ios.ios_command` module. It retrieves the IOS version, displays a brief overview of IP interfaces, and captures the router's running configuration.

4. Print and Save Output: The output of the executed commands is registered, printed for debugging purposes, and saved to a specified destination. This allows for documentation and backup of the router's configuration.

In summary, this role automates the initial configuration and maintenance of Cisco routers in a network, focusing on interfaces and routing, and it collects and saves relevant information for future reference.

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

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
