Role Name
=========

Install Node.js from NodeSource

Requirements
------------

Role Variables
--------------

node_version: Node.js version to install

Dependencies
------------

Example Playbook
----------------

    - hosts: servers
      roles:
        - {
            role: oscbco.install_nodejs,
            node_version: 10.x
          }

License
-------

MIT

Author Information
------------------

oscbco.dev
