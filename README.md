ansible-role-logiops
=========

This role can be used to install and configure the [logiops](https://github.com/PixlOne/logiops) drivers on Linux

Requirements
------------

You need to have a logid configuration (logid.cfg) present under files/logid.cfg. An example is already present, with a detailed guide on how to make one at the project's [wiki](https://github.com/PixlOne/logiops/wiki)

Role Variables
--------------

Please inspect defaults/main.yml and vars/main.yml for the possible variables - they should be self-explanatory.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      vars:
        user: "robinopletal"
        logiops_source_repo_dir: "home/{{ user }}/Programs"
        upgrade_system: true

      roles:
         - role: ansible-role-logiops

License
-------

MIT
